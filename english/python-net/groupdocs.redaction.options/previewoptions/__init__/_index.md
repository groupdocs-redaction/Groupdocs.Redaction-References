---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new PreviewOptions instance."
type: docs
url: /python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initializes a new PreviewOptions instance. The output stream will be closed after use.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Creates a stream for a specific page preview. |

## __init__ {#create_page_stream-release_page_stream}

Initializes a new PreviewOptions instance, causing the output stream to be returned to the client for further use.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Creates a stream for a specific page preview. |
| release_page_stream | `ReleasePageStream` | Notifies that the page preview generation is done and gets output stream. |

### See Also
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
