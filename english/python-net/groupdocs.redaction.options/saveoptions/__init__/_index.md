---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance with default settings: rasterize to PDF is False and add suffix is False."
type: docs
url: /python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance with default settings: rasterize to PDF is False and add suffix is False.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions

with Redactor("sample.docx") as redactor:
    # Apply redactions here
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Saved to {result_path}")
```

## __init__ {#rasterize_to_pdf-suffix}

Initializes a new SaveOptions instance with given parameters.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, if all pages in the document need to be converted to images and put in a single PDF file. |
| suffix | `str` | Text added to the end of the file name; if not empty also sets `add_suffix` to True. |

### Example

```python
from groupdocs.redaction.options import SaveOptions

# Save with pages rasterized to a single PDF and add a suffix to the filename
options = SaveOptions(rasterize_to_pdf=True, suffix="redacted")
```

### See Also
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
