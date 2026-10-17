---
title: "تعديلات جداول البيانات"
linkTitle: "Spreadsheet redactions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيف يسمح Python redaction API بإخفاء البيانات الحساسة أو الخاصة من صيغ مستندات جداول البيانات XLS و XLSX و ODS وغيرها."
type: docs
url: /ar/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


يتيح GroupDocs.Redaction إخفاء البيانات الحساسة أو الخاصة من صيغ مستندات جداول البيانات XLS و XLSX و ODS وغيرها. راجع القائمة الكاملة في مقالة [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # حمّل جدول البيانات الذي سيُخفى
    with Redactor("./sample.xlsx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` هو ملف العينة المستخدم في هذا المثال. اضغط [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) لتنزيله.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
