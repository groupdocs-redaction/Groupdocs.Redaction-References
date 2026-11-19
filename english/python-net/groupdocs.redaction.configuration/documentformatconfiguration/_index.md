---
title: DocumentFormatConfiguration class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a type reference for DocumentFormatInstance-derived class and supported file extensions list for faster format detection."
type: docs
url: /python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Represents a type reference for [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-derived class and supported file extensions list for faster format detection.

Learn more

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/python-net/extend-supported-extensions-list/

The DocumentFormatConfiguration type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initializes a new instance of DocumentFormatConfiguration class. |

### Methods
| Method | Description |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Checks if a given file extension can be handled as DocumentType. |

### Properties
| Property | Description |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | The type of a class inheriting from [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | The comma‑separated list of file extensions (e.g., ".pdf"), case‑insensitive, used to filter supported formats. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | The data required for [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) initialization. |

### Example

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Open .dump files with the plain-text format handler
config = RedactorConfiguration.get_instance()
text_format = config.find_format(".txt")  # a DocumentFormatConfiguration
text_format.extension_filter = text_format.extension_filter + ",.dump"
```

### See Also
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
