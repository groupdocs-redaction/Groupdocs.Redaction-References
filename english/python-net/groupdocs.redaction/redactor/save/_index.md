---
title: save method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Saves the document to a file with the following options: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Saves the document to a file with the following options: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Saves the document to a file.

```python
def save(self, save_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| save_options | `SaveOptions` | Options to add suffix or rasterize. |

**Returns:** Path to redacted document.

### Example

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Specify the redaction options
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Load the document to be redacted
    with Redactor("./sample.docx") as redactor:
        # Apply the redaction
        redactor.apply(ex_red)

        # Save the redacted document in its original format with a date suffix
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Saves the document to a stream, including custom location.

```python
def save(self, document, rasterization_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Target stream. |
| rasterization_options | `RasterizationOptions` | Options to rasterize or not and to specify pages for rasterization. |

### Example

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # configure rasterization to process only the first slide
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # the BytesIO object now contains the saved document
    data = stream.getvalue()
```

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
