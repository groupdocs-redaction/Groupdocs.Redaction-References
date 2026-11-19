---
title: release_page_stream property
second_title: GroupDocs.Redaction for Python via .NET API References
description: "The page preview completion delegate."
type: docs
url: /python-net/groupdocs.redaction.options/previewoptions/release_page_stream/
is_root: false
weight: 2050
---


## release_page_stream property

The page preview completion delegate.

The delegate is invoked after a page preview has been rendered. It receives the page number (`int`) and the stream (`io.RawIOBase`) that was returned by the `create_page_stream` delegate, allowing the caller to close, inspect, or otherwise process the image data.

### Definition:
```python
@property
def release_page_stream(self):
    ...
@release_page_stream.setter
def release_page_stream(self, value):
    ...
```

### See Also
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
