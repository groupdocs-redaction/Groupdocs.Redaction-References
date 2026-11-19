---
title: save method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Saves the document to a file using the provided SaveOptions."
type: docs
url: /python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1050
---


## save

Saves the document to a file using the provided [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/). By default, `AddSuffix` is set to `True` and `RasterizeToPDF` is set to `True`.

```python
def save(self):
    ...
```

**Returns:** str: Path to the redacted document.

## save {#save_options}

Saves the document to a file.

```python
def save(self, save_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| save_options | `SaveOptions` | Options to add suffix or rasterize. |

**Returns:** str: Path to redacted document.

### Example

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_in_original_format():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("Emily Johnson", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")
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
import os
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    # Set rasterization options (e.g., first slide only)
    rasterization_options = RasterizationOptions()
    rasterization_options.page_index = 0
    rasterization_options.page_count = 1
    rasterization_options.compliance = PdfComplianceLevel.PDF_A1A

    # Save the redacted document to a file stream
    output_path = os.path.join(r"C:\Temp", "PresentationFirstSlide.pdf")
    with open(output_path, "w+b") as stream:  # read/write: PDF/A conversion reads it back
        redactor.save(stream, rasterization_options)
```

## save {#document-save_options}

Saves the document to the specified stream.

```python
def save(self, document, save_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The target stream. |
| save_options | `SaveOptions` | The save options that control rasterization, the output file name suffix, and document-specific save settings. |

### Example

```python
import io
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions

with Redactor("document.docx") as redactor:
    # Apply redactions as needed
    buf = io.BytesIO()
    redactor.save(buf, SaveOptions(rasterize_to_pdf=False))
    data = buf.getvalue()
```

### Aliases

These names call `save` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `save_stream` | `save_stream(document, rasterization_options)`<br>`save_stream(document, save_options)` |
| `save_streams` | `save_streams(document, rasterization_options)`<br>`save_streams(document, save_options)` |
| `save_save_options` | `save_save_options(save_options)` |

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
