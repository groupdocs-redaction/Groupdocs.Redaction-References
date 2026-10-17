---
title: "طريقة generate_preview"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة.

يتم إنشاء المعاينة وفقًا للإعدادات المحددة في `preview_options`، والتي تشمل تنسيق الصورة، الأبعاد، نطاق الصفحات، والنداءات لإنشاء وإطلاق تدفقات الصفحات.

```python
def generate_preview(self, preview_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| preview_options | `PreviewOptions` | خصائص الصورة وإعدادات نطاق الصفحات. |

### مثال

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # يعيد تدفق ملف قابل للكتابة لصورة المعاينة للصفحة المحددة.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # يُستدعى بعد كتابة صورة المعاينة.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### انظر أيضًا
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
