---
title: DocumentFormatConfiguration class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---

## DocumentFormatConfiguration class

Represents a type reference for [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance)-derived class and supported file extensions list for faster format detection.



The DocumentFormatConfiguration type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/#) | Initializes a new instance of DocumentFormatConfiguration class. |


### Properties
| Property | Description |
| :- | :- |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter) | Gets or sets a comma (",") delimited list of file extensions (for example ".pdf"), case insensitive. |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type) | Gets or sets the type of a class, inheriting from [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance). |


### Methods
| Method | Description |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#str) | Checks if a given file extension can be handled as DocumentType. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to set properties for a custom format configuration.

### See Also
* module [`groupdocs.redaction.configuration`](..)
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance)
