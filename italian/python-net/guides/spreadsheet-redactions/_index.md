---
title: "Redazioni di fogli di calcolo"
linkTitle: "Spreadsheet redactions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra come l'API di redazione Python consenta di redigere dati di natura sensibile o privata dai tuoi formati di documento foglio di calcolo XLS, XLSX, ODS e altri."
type: docs
url: /it/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction consente di redigere dati di natura sensibile o privata dai tuoi formati di documento foglio di calcolo XLS, XLSX, ODS e altri. Vedi l'elenco completo nell'articolo [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Carica il foglio di calcolo da redigere
    with Redactor("./sample.xlsx") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` è il file di esempio usato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) per scaricarlo.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
