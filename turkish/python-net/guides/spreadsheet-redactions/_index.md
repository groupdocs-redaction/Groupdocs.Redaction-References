---
title: "Elektronik tablo redaksiyonları"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, Python redaksiyon API'sinin XLS, XLSX, ODS elektronik tablo belge formatlarınız ve diğerlerinden hassas veya özel nitelikteki verileri nasıl redakte edebileceğini gösterir."
type: docs
url: /tr/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction, XLS, XLSX, ODS elektronik tablo belge formatlarınız ve diğerlerinden hassas veya özel nitelikteki verileri redakte etmenizi sağlar. Tam listeyi [supported document formats]() makalesinde görebilirsiniz.

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Redakte edilecek elektronik tabloyu yükleyin
    with Redactor("./sample.xlsx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) tıklayın.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
