---
title: RedactorConfiguration class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides access to a list of supported formats, built-in and custom user formats."
type: docs
url: /python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Provides access to a list of supported formats, built-in and custom user formats.

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/python-net/extend-supported-extensions-list/

The RedactorConfiguration type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Finds format configurations for a given file extension. |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Provides a singleton instance with the default configuration of built-in formats. |

### Properties
| Property | Description |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | The list of recognized formats, see [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Example

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Open .dump files with the plain-text format handler
config = RedactorConfiguration.get_instance()
text_format = config.find_format(".txt")  # a DocumentFormatConfiguration
text_format.extension_filter = text_format.extension_filter + ",.dump"
```

```python
from groupdocs.redaction.configuration import RedactorConfiguration

config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### See Also
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
