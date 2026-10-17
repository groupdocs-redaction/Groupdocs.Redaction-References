---
title: "Redaksi spreadsheet"
linkTitle: "Spreadsheet redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan bagaimana API redaksi Python memungkinkan untuk meredaksi data yang bersifat sensitif atau pribadi dari format dokumen spreadsheet XLS, XLSX, ODS Anda, dan lainnya."
type: docs
url: /id/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction memungkinkan meredaksi data yang bersifat sensitif atau pribadi dari format dokumen spreadsheet XLS, XLSX, ODS Anda, dan lainnya. Lihat daftar lengkap pada artikel [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Muat spreadsheet yang akan diredaksi
    with Redactor("./sample.xlsx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` adalah file contoh yang digunakan dalam contoh ini. Klik [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) untuk mengunduhnya.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
