---
title: RasterizationOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 40
---

## RasterizationOptions class

Provides options for converting files into PDF.



The RasterizationOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/#) | Initializes a new instance. |


### Properties
| Property | Description |
| :- | :- |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled) | Gets or sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index) | Gets or sets the index of the first page (0-based) to convert into PDF. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count) | Gets or sets the number of pages to be converted into PDF. |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance) | Gets or sets the PDF Compliance level. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options) | Gets an indicator, which is true if advanced rasterization options are set. |


### Methods
| Method | Description |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#groupdocs.redaction.options.AdvancedRasterizationOptions) | You can use this method to register an advanced rasterization option to apply. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to set options for the rasterization process.

### See Also
* module [`groupdocs.redaction.options`](..)
