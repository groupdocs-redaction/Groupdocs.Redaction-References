---
title: "طريقة save"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

يحفظ المستند إلى ملف.

```python
def save(self, save_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| save_options | `SaveOptions` | خيارات لإضافة لاحقة أو تحويل إلى نقطية. |

**Returns:** Path to redacted document.

### مثال

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        redactor.apply(ex_red)

        # احفظ المستند المُحَرَّف بصيغته الأصلية مع لاحقة تاريخية.
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

يحفظ المستند إلى تدفق، بما في ذلك الموقع المخصص.

```python
def save(self, document, rasterization_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| document | `io.RawIOBase` | المسار الهدف. |
| rasterization_options | `RasterizationOptions` | خيارات لتحويل إلى نقطية أو لا وتحديد الصفحات للتحويل. |

### مثال

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # تكوين التحويل إلى نقطية لمعالجة الشريحة الأولى فقط.
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # كائن BytesIO الآن يحتوي على المستند المحفوظ
    data = stream.getvalue()
```

### انظر أيضًا
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
