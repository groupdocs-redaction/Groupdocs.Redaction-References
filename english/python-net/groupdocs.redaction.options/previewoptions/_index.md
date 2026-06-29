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

The class allows specifying the preview format, image dimensions, page numbers, and delegates that create and optionally release streams for each generated page.

The PreviewOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initializes a new PreviewOptions instance. The output stream will be closed after use. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initializes a new PreviewOptions instance, causing the output stream to be returned to the client for further use. |

### Properties
| Property | Description |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | The page stream creation delegate. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | The page preview height. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | The page numbers to generate preview. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | The preview image format. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | The page preview completion delegate. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | The page preview width. |

### Example

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Create a file for the preview image of the given page
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
