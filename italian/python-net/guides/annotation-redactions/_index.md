---
title: "Redazioni di annotazione"
linkTitle: "Annotation redactions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra l'implementazione della redazione di annotazione per documenti di diversi formati come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri."
type: docs
url: /it/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Con l'API di GroupDocs.Redaction puoi applicare redazioni di annotazione per documenti di diversi formati come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri. Vedi l'elenco completo nell'articolo [formati di documento supportati]().

GroupDocs.Redactions fornisce un'API flessibile che consente di rimuovere dati sensibili dal testo delle annotazioni, o di rimuovere completamente le annotazioni mediante un'espressione regolare.

## Remove annotations (comments etc)

Puoi usare GroupDocs.Redaction per rimuovere tutti o specifici commenti e altre annotazioni dal documento. Ad esempio, possiamo rimuovere tutti i commenti dal documento, contenenti testi come \"use\", \"show\" o \"describe\" nel corpo:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Specifica le opzioni di redazione per eliminare le annotazioni che corrispondono al modello
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Carica il documento da redigere
    with Redactor("./annotated.xlsx") as redactor:
        # Applica la redazione
        result = redactor.apply(a_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` è il file di esempio usato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) per scaricarlo.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Puoi usare il costruttore senza argomenti per rimuovere tutte le annotazioni all'interno del documento.

## Redact annotations

Invece di rimuovere tutte o specifiche annotazioni, è possibile rimuovere i dati sensibili dal testo dell'annotazione. Ad esempio, possiamo rimuovere tutti i riferimenti a "John" nel documento fornito, per esempio:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Specifica le opzioni di redazione: modello di ricerca e stringa di sostituzione
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Carica il documento da redigere
    with Redactor("./annotated.xlsx") as redactor:
        # Applica la redazione
        result = redactor.apply(a_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` è il file di esempio usato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) per scaricarlo.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
