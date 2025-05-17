---
title: Redactor class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/redactor/
is_root: false
weight: 100
---

## Redactor class

Represents a main class that controls document redaction process, allowing to open, redact and save documents.



The Redactor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using file path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.RawIOBase) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str-groupdocs.redaction.options.LoadOptions) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str-groupdocs.redaction.options.LoadOptions-groupdocs.redaction.options.RedactorSettings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path and settings. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.RawIOBase-groupdocs.redaction.options.LoadOptions) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.RawIOBase-groupdocs.redaction.options.LoadOptions-groupdocs.redaction.options.RedactorSettings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream and settings. |


### Methods
| Method | Description |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#groupdocs.redaction.Redaction) | Applies a redaction to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#list) | Applies a set of redactions to the document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#groupdocs.redaction.RedactionPolicy) | Applies a redaction policy to the document. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#) | Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#groupdocs.redaction.options.SaveOptions) | Saves the document to a file. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#io.RawIOBase-groupdocs.redaction.options.RasterizationOptions) | Saves the document to a stream, including custom location. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#groupdocs.redaction.options.PreviewOptions) | Generates preview images of specific pages in a given image format. |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/#) | Gets the general information about the document - size, page count, etc. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates applying a single redaction to the document.


The following example demonstrates applying a list of redactions to the document.


The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.


The following example demonstrates how to open a password-protected documents using LoadOptions.


The following example demonstrates how to save a document using SaveOptions.

### See Also
* module [`groupdocs.redaction`](..)
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable)
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor)
