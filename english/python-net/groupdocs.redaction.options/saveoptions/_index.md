---
title: SaveOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 60
---

## SaveOptions class

Provides options for changing an output file name and/or converting the document to image-based PDF (rasterization).



The SaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#) | Initializes a new instance with defaults: rasterize to PDF - false, add suffix - false. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#bool-str) | Initializes a new instance with given parameters. |


### Properties
| Property | Description |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix) | Gets or sets a value indicating whether the file name needs to be changed before saving. False by default. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix) | Gets or sets a custom suffix for output file name. If it is not specified, the [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions) constant will be used. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf) | Gets or sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization) | Gets the rasterization settings. |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix) | Represents default suffix value, which is "Redacted". |



### Remarks 


**Learn more** |
|
 |
 |
 |
 |
 |
 |

### Example 


The following example demonstrates how to save a document using SaveOptions.

### See Also
* module [`groupdocs.redaction.options`](..)
