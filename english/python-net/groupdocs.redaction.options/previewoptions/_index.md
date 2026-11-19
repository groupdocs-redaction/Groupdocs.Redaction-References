---
title: PreviewOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides options to set requirements and stream delegates for preview generation."
type: docs
url: /python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Provides options to set requirements and stream delegates for preview generation.

Use this class with [`Redactor.generate_preview`](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/) to render document pages to image streams.

The PreviewOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initializes a new PreviewOptions instance, causing the output stream to be closed. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initializes a new PreviewOptions instance, causing the output stream to be returned to the client for further use. |

### Properties
| Property | Description |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | The page stream creation delegate used to obtain a writable `io.RawIOBase` stream for each rendered page. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | The page preview height. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | The page numbers to generate preview. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | The preview image format. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | The page preview completion delegate. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | The page preview width. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import PreviewOptions

def get_document_page_preview():
    def create_page_stream(page_number):
        return open(f"preview_page_{page_number}.png", "wb")

    with Redactor("./multipage_sample.docx") as redactor:
        options = PreviewOptions(create_page_stream)
        options.width = 480
        options.height = 640
        options.page_numbers = [1]
        options.preview_format = PreviewOptions.PreviewFormats.PNG
        redactor.generate_preview(options)
        print("The preview of page 1 is saved to preview_page_1.png")
```

### Guides
Task guides that use `PreviewOptions`:

* [Get document page preview](/redaction/python-net/guides/get-document-page-preview/)

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
