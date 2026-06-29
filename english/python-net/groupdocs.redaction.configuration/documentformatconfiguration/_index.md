---
title: DocumentFormatConfiguration class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a type reference for DocumentFormatInstance-derived class and a list of supported file extensions for faster format detection."
type: docs
url: /python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Represents a type reference for [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-derived class and a list of supported file extensions for faster format detection.

Learn more

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

The DocumentFormatConfiguration type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initializes a new instance of DocumentFormatConfiguration. |

### Methods
| Method | Description |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Checks if a given file extension can be handled as DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Properties
| Property | Description |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | The type of a class inheriting from [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | The comma‑delimited list of file extensions (for example ".pdf"), case‑insensitive. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | The data required for [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) initialization. |

### Example

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Create a custom format configuration
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### See Also
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
