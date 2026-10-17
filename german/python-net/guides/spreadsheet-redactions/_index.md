---
title: "Tabellenkalkulation-Redaktionen"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie die Python‑Redaction‑API Daten sensibler oder privater Art aus Ihren XLS-, XLSX‑ und ODS‑Tabellenkalkulationsformaten sowie anderen Formaten redigieren kann."
type: docs
url: /de/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction ermöglicht das Redigieren von Daten sensibler oder privater Art aus Ihren XLS-, XLSX‑ und ODS‑Tabellenkalkulationsformaten sowie anderen Formaten. Siehe die vollständige Liste im Artikel [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laden Sie die zu redigierende Tabellenkalkulation
    with Redactor("./sample.xlsx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` ist die in diesem Beispiel verwendete Beispieldatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx), um sie herunterzuladen.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
