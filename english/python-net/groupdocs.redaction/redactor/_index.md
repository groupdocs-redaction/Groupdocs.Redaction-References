---
title: Redactor class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents the main class that controls the document redaction process, allowing opening, redacting, and saving documents."
type: docs
url: /python-net/groupdocs.redaction/redactor/
is_root: false
weight: 120
---


## Redactor class

Represents the main class that controls the document redaction process, allowing opening, redacting, and saving documents.

Learn more
- More details about applying redactions: <https://docs.groupdocs.com/redaction/python-net/redaction-basics/>
- More advanced redaction topics: <https://docs.groupdocs.com/redaction/python-net/advanced-usage/>

The Redactor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initializes a new Redactor instance using a file path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initializes a new Redactor instance using a document stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initializes a new Redactor instance for a password-protected document using its path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using its path and settings. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initializes a new Redactor instance for a password‑protected document using a stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using a stream and optional settings. |

### Methods
| Method | Description |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Applies a redaction to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Applies a set of redactions to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Applies a redaction policy to the document. |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Releases resources. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Generates preview images of specific pages in a given image format. |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Retrieves general information about the document, such as size and page count. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Saves the document to a file using the provided [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/). By default, `AddSuffix` is set to `True` and `RasterizeToPDF` is set to `True`. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Saves the document to a file. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Saves the document to a stream, including custom location. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-save_options) | Saves the document to the specified stream. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Open a PDF document
with Redactor("document.pdf") as redactor:
    # Remove the first page
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    # Save the redacted document (overwrites the original file)
    redactor.save()
```

### Guides
Task guides that use `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Quick Start Guide](/redaction/python-net/guides/quick-start-guide/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Get document page preview](/redaction/python-net/guides/get-document-page-preview/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Use redaction callback](/redaction/python-net/guides/use-redaction-callback/)
* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Load with file type](/redaction/python-net/guides/load-with-file-type/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)
* [Save Word with OOXML compliance](/redaction/python-net/guides/save-word-with-ooxml-compliance/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
