---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz mit Standardeinstellungen: rasterizetopdf ist False und addsuffix ist False."
type: docs
url: /de/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue Instanz mit Standardeinstellungen: rasterize_to_pdf ist False und add_suffix ist False.

```python
def __init__(self):
    ...
```

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Initialisiert eine neue Instanz mit angegebenen Parametern.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, wenn alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden müssen. |
| suffix | `str` | Dieser Text wird an das Ende des Dateinamens angehängt; wenn er nicht leer ist, wird außerdem `add_suffix` auf True gesetzt. |

### Beispiel

```python
from groupdocs.redaction.options import SaveOptions

# Speicheroptionen mit Standardeinstellungen erstellen
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Siehe auch
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
