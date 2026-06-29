---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance with default settings: rasterizetopdf is False and addsuffix is False."
type: docs
url: /python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance with default settings: rasterize_to_pdf is False and add_suffix is False.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Initializes a new instance with given parameters.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, if all pages in the document need to be converted to images and put in a single PDF file. |
| suffix | `str` | This text will be added to the end of the file name; if not empty also sets `add_suffix` to True. |

### Example

```python
from groupdocs.redaction.options import SaveOptions

# Create save options with default settings
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### See Also
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
