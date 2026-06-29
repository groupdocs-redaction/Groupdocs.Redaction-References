---
title: generate_preview method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Generates preview images of specific pages in a given image format."
type: docs
url: /python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Generates preview images of specific pages in a given image format.

The preview is produced according to the settings defined in `preview_options`, which include image format, dimensions, page range, and callbacks for creating and releasing page streams.

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

def create_page_stream(page_number):
    # Returns a writable file stream for the preview image of the given page.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Called after the preview image has been written.
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

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
