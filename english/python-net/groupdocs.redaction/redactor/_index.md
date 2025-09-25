---
title: Redactor class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 100
url: /groupdocs.redaction/redactor/
is_root: false
---

## Redactor class

Represents a main class that controls document redaction process, allowing to open, redact and save documents.



The Redactor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, file_path)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using file path. |
| [`__init__(self, document)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.rawiobase) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using stream. |
| [`__init__(self, file_path, load_options)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str-groupdocs.redaction.options.loadoptions) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path. |
| [`__init__(self, file_path, load_options, settings)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#str-groupdocs.redaction.options.loadoptions-groupdocs.redaction.options.redactorsettings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path and settings. |
| [`__init__(self, document, load_options)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.rawiobase-groupdocs.redaction.options.loadoptions) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream. |
| [`__init__(self, document, load_options, settings)`](/redaction/python-net/groupdocs.redaction/redactor/__init__/#io.rawiobase-groupdocs.redaction.options.loadoptions-groupdocs.redaction.options.redactorsettings) | Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream and settings. |


### Methods
| Method | Description |
| :- | :- |
| [`apply(self, redaction)`](/redaction/python-net/groupdocs.redaction/redactor/apply/#groupdocs.redaction.redaction) | Applies a redaction to the document. |
| [`apply(self, redactions)`](/redaction/python-net/groupdocs.redaction/redactor/apply/#list) | Applies a set of redactions to the document. |
| [`apply(self, policy)`](/redaction/python-net/groupdocs.redaction/redactor/apply/#groupdocs.redaction.redactionpolicy) | Applies a redaction policy to the document. |
| [`save(self)`](/redaction/python-net/groupdocs.redaction/redactor/save/#) | Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true. |
| [`save(self, save_options)`](/redaction/python-net/groupdocs.redaction/redactor/save/#groupdocs.redaction.options.saveoptions) | Saves the document to a file. |
| [`save(self, document, rasterization_options)`](/redaction/python-net/groupdocs.redaction/redactor/save/#io.rawiobase-groupdocs.redaction.options.rasterizationoptions) | Saves the document to a stream, including custom location. |
| [`generate_preview(self, preview_options)`](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#groupdocs.redaction.options.previewoptions) | Generates preview images of specific pages in a given image format. |
| [`get_document_info(self)`](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/#) | Gets the general information about the document - size, page count, etc. |



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
