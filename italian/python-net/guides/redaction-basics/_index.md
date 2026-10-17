---
title: "Nozioni di base sulla redazione"
linkTitle: "Redaction basics"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra come gli sviluppatori Python possano applicare la redazione di metadati, immagini, annotazioni e testo nei loro documenti. È supportata un'ampia gamma di formati di documento, come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri."
type: docs
url: /it/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction supporta un set efficace di funzionalità di redazione dei documenti. Consente di applicare redazioni per [text](), [metadata](), [annotations](), [images]().

È supportata un'ampia gamma di formati di documento, come: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri. Consulta l'elenco completo dei formati supportati nell'articolo [supported document formats]().

## Redaction types

GroupDocs.Redaction include i seguenti tipi di redazione:

| Tipo | Descrizione | Classi |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

L'applicazione della redazione a un documento avviene tramite il metodo [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . Di conseguenza, si riceve un'istanza di [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) contenente una voce di registro per ogni redazione applicata. La voce contiene un riferimento all'istanza [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) includendo le sue opzioni, lo stato dell'operazione (vedi sotto) e le descrizioni testuali, se applicabili. Se almeno una redazione fallisce, vedrai [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Salva il documento redatto accanto al file sorgente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` è il file di esempio usato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Tutti i possibili stati dell'enumerazione [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) sono elencati in questa tabella:

| Stato | Descrizione | Motivi possibili |
| --- | --- | --- |
| *Applicato* | La redazione è stata applicata completamente e con successo | Tutte le operazioni all'interno del processo di redazione sono state applicate con successo |
| *ParzialmenteApplicato* | La redazione è stata applicata solo a una parte delle sue corrispondenze | 1) I limiti di prova per le sostituzioni sono stati superati2) Almeno una modifica è stata rifiutata dall'utente |
| *Ignorato* | La redazione è stata ignorata (non applicata) | 1) I limiti di prova per le redazioni sono stati superati2) La redazione non può essere applicata a questo tipo di documento3) Tutte le sostituzioni sono state rifiutate dall'utente e non sono state apportate modifiche |
| *Fallito* | La redazione è fallita con eccezione | Si è verificata un'eccezione durante il processo di redazione |

Per informazioni dettagliate è necessario iterare le voci del registro di redazione in [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) e controllare la proprietà [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) di tutti gli elementi con stato diverso da *Applicato*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Per impostazione predefinita, il documento redatto viene salvato in formato PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Esporta tutte le redazioni fallite o ignorate
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Puoi applicare quante redazioni desideri in una singola chiamata al metodo [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , poiché il suo overload accetta un array di redazioni e una politica di redazione. In questo caso, le redazioni saranno applicate nello stesso ordine in cui compaiono nell'array. Come alternativa alla specifica dei set di redazione nel tuo codice, puoi creare un file XML con la politica di redazione, come descritto [qui]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Fornisci un elenco di redazioni da applicare in ordine
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica l'elenco delle redazioni
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Per impostazione predefinita, il documento redatto viene salvato in formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Esporta tutte le redazioni fallite o ignorate
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` è il file di esempio usato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) per scaricarlo.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
