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
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import PreviewOptions

def create_page_stream(page_number):
    return open(f"preview_page_{page_number}.png", "wb")

with Redactor("./multipage_sample.docx") as redactor:
    options = PreviewOptions(create_page_stream)
    options.width = 480
    options.height = 640
    options.page_numbers = [1]
    options.preview_format = PreviewOptions.PreviewFormats.PNG
    redactor.generate_preview(options)
    print("Preview saved to preview_page_1.png")
```

### Aliases

These names call `generate_preview` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `generate_preview_preview_options` | `generate_preview_preview_options(preview_options)` |

### See Also
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
