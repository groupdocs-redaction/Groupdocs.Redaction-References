---
title: generate_preview method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Generates preview images of specific pages in a given image format."
type: docs
url: /python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Generates preview images of specific pages in a given image format.

```python
def generate_preview(self, preview_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Image properties and page range settings. |

### Example

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

### See Also
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
