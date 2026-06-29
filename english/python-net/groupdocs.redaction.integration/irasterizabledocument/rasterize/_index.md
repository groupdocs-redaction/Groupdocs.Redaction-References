---
title: rasterize method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Saves the document to a stream as a PDF."
type: docs
url: /python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

Saves the document to a stream as a PDF.

```python
def rasterize(self, output):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Target stream. |

## rasterize {#output-options}

Saves the document to a stream as a PDF with page range and compliance options.

```python
def rasterize(self, output, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Target stream. |
| options | `RasterizationOptions` | PDF conversion options. |

### See Also
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
