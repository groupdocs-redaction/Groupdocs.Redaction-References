---
title: "Spreadsheet-redacties"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe de Python redactie‑API gevoelige of privégegevens kan redigeren uit uw XLS-, XLSX- en ODS‑spreadsheetdocumentformaten en andere."
type: docs
url: /nl/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction maakt het mogelijk om gevoelige of privégegevens te redigeren uit uw XLS-, XLSX- en ODS‑spreadsheetdocumentformaten en andere. Zie de volledige lijst in het artikel [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laad de spreadsheet die moet worden geredigeerd
    with Redactor("./sample.xlsx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(ex_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) om het te downloaden.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
