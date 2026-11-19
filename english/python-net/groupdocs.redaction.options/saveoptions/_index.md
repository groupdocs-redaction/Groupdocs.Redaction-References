---
title: SaveOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides options for changing an output file name and/or converting the document to image‑based PDF (rasterization)."
type: docs
url: /python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Provides options for changing an output file name and/or converting the document to image‑based PDF (rasterization).

Learn more
- [Save with default options](https://docs.groupdocs.com/redaction/python-net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/python-net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/python-net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/python-net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/python-net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/python-net/save-to-stream/)

The SaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Initializes a new instance with default settings: rasterize to PDF is False and add suffix is False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Initializes a new SaveOptions instance with given parameters. |

### Properties
| Property | Description |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | The file name will be changed before saving when set to True. False by default. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | The rasterization settings. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | The rasterize_to_pdf property indicates whether all pages in the document are converted to images and placed in a single PDF file. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | The custom suffix for the output file name. If not specified, the [`SaveOptions.save_suffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) constant is used. |
| [wordprocessing_save_options](/redaction/python-net/groupdocs.redaction.options/saveoptions/wordprocessing_save_options/) | The save options specific to word processing documents. |

### Fields
| Field | Description |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Represents default suffix value, which is "Redacted". |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("./sample.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions("[personal]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    options.redacted_file_suffix = "redacted"
    result_path = redactor.save(options)
    print(f"Document saved to {result_path}")
```

### Guides
Task guides that use `SaveOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Quick Start Guide](/redaction/python-net/guides/quick-start-guide/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Load with file type](/redaction/python-net/guides/load-with-file-type/)
* [Save Word with OOXML compliance](/redaction/python-net/guides/save-word-with-ooxml-compliance/)

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
