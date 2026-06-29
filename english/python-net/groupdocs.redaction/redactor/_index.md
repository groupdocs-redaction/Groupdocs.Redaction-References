---
title: Redactor class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a main class that controls document redaction process, allowing to open, redact and save documents."
type: docs
url: /python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Represents a main class that controls document redaction process, allowing to open, redact and save documents.

Learn more
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

The Redactor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initializes a new Redactor instance using a file path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) using a stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using its path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initializes a new Redactor instance for a password‑protected document using its path and settings. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initializes a new Redactor instance for a password‑protected document using a stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using a stream and settings. |

### Methods
| Method | Description |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Applies a redaction to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Applies a set of redactions to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Applies a redaction policy to the document. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Releases resources. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Generates preview images of specific pages in a given image format. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Retrieves the general information about the document, such as size and page count. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Saves the document to a file with the following options: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Saves the document to a file. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Saves the document to a stream, including custom location. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Open a document and remove the first page
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Task guides that use `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
