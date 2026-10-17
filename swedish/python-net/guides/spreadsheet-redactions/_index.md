---
title: "Kalkylbladsredigeringar"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel visar hur Python redaction API möjliggör att redigera data av känslig eller privat natur från dina XLS, XLSX, ODS kalkylbladsdokumentformat och andra."
type: docs
url: /sv/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction möjliggör att redigera data av känslig eller privat natur från dina XLS, XLSX, ODS kalkylbladsdokumentformat och andra. Se fullständig lista i artikeln [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Läs in kalkylbladet som ska redigeras
    with Redactor("./sample.xlsx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` är exempelfilen som används i detta exempel. Klicka på [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) för att ladda ner den.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
