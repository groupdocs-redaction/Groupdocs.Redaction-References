---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new PreviewOptions instance, causing the output stream to be closed."
type: docs
url: /python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initializes a new PreviewOptions instance, causing the output stream to be closed.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Creates a stream for a specific page preview. |

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
    ```

## __init__ {#create_page_stream-release_page_stream}

Initializes a new PreviewOptions instance, causing the output stream to be returned to the client for further use.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Callable[[int], io.RawIOBase] – Creates a stream for a specific page preview. |
| release_page_stream | `ReleasePageStream` | Callable[[int, io.RawIOBase], None] – Notifies that the page preview generation is done and receives the output stream. |

### See Also
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
