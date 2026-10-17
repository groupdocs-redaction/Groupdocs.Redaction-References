---
title: "Redazioni di metadati"
linkTitle: "Metadata redactions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra come l'API di redazione Python consenta di sostituire o rimuovere i metadati usando filtri o ricerca con espressioni regolari."
type: docs
url: /it/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Con l'API GroupDocs.Redaction puoi applicare redazioni di metadati a documenti di diversi formati come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri. Vedi l'elenco completo nell'articolo [supported document formats]().

GroupDocs.Redactions fornisce un'API flessibile che consente di sostituire o rimuovere i metadati usando filtri o ricerca con espressioni regolari.

## Filter metadata

La funzionalità di base per tutte le redazioni, derivata dalla classe base [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/), è *metadata filtering* ed è obbligatoria per le redazioni di metadati. Utilizza l'enumerazione con flag [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), contenente elementi per le voci di metadati più frequenti. È possibile impostare il filtro su *All*, o su qualsiasi combinazione di metadati. Ad esempio, l'esempio seguente imposta il filtro su *Author*, *Manager* e *NameOfApplication* - per la redazione testuale o per la loro pulizia:

```python
# redazione derivata da MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Di seguito è la tabella con l'elenco completo degli elementi di [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Filtro | Valore numerico | Descrizione |
| --- | --- | --- |
| *None* | 0 | Impostazione filtro vuoto, non corrisponde a nessun elemento di metadati |
| *Author* | 1 | Autore del documento |
| *Categoria* | 2 | Categoria del documento |
| *Commenti* | 4 | Commento del documento |
| *Azienda* | 8 | Azienda dell'Autore |
| *ContentStatus* | 16 | Stato del contenuto |
| *CreatedTime* | 32 | Ora di creazione |
| *HyperlinkBase* | 64 | Base del collegamento ipertestuale |
| *LastPrinted* | 128 | Data e ora dell'ultima stampa |
| *LastSavedBy* | 256 | Ultimo salvataggio da parte dell'utente |
| *LastSavedTime* | 1024 | Data e ora dell'ultimo salvataggio |
| *NameOfApplication* | 2048 | Nome dell'applicazione in cui è stato creato il documento |
| *Manager* | 4096 | Nome del responsabile dell'autore |
| *RevisionNumber* | 8192 | Numero di revisione |
| *Subject* | 16384 | Oggetto del documento |
| *Template* | 32768 | Nome del modello del documento |
| *Title* | 65536 | Titolo del documento |
| *TotalEditingTime* | 131072 | Tempo totale di modifica |
| *Versione* | 262144 | Versione del documento |
| *Descrizione* | 524288 | Descrizione del documento |
| *Parole chiave* | 1048576 | Parole chiave del documento |
| *TipoContenuto* | 2097152 | Tipo di contenuto |
| *Tutti* | 2147483647 | Tutti i tipi di elementi dei metadati |

## Clean metadata

È possibile sostituire tutti o specifici metadati nel documento con valori vuoti (blank o minimi) utilizzando la classe [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/). L'esempio seguente elimina tutte le proprietà del documento:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Specifica le opzioni di redazione per cancellare tutti i metadati
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(met_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

È possibile specificare [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) o utilizzare il costruttore predefinito per cancellare tutti i metadati nel documento specificato, Custom - per cancellare tutte le voci di metadati personalizzati.

## Redact metadata

È possibile utilizzare [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) per rimuovere dati sensibili dai metadati del documento usando espressioni regolari. Ad esempio, possiamo rimuovere qualsiasi menzione di \"Company Ltd.\":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Specifica le opzioni di redazione: modello di ricerca e stringa di sostituzione
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(met_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Il primo argomento è un'espressione regolare, il secondo è una stringa di sostituzione. È inoltre possibile impostare l'ambito della redazione impostando il filtro, ad es. a [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - lascerà le corrispondenze delle espressioni regolari non modificate in tutti gli elementi dei metadati, eccetto la proprietà \"Company\":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Specifica le opzioni di redazione: modello di ricerca e stringa di sostituzione
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Limita l'ambito della redazione solo all'elemento di metadati Company
    met_red.filter = MetadataFilters.COMPANY

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(met_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Tutte le redazioni dei metadati si applicano a ciascun elemento di metadati separatamente e, anche se la redazione di un elemento di metadati fallisce, il resto degli elementi verrà aggiornato. È possibile trovare un elenco di elementi di metadati falliti, saltati (rifiutati) e le relative ragioni nella proprietà [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) di [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
