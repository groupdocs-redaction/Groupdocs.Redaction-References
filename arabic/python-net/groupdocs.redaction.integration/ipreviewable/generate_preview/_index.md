---
title: "طريقة generate_preview"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### انظر أيضًا
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
