---
title: find_format method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Finds format configurations for a given file extension."
type: docs
url: /python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Finds format configurations for a given file extension.

```python
def find_format(self, file_extension):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_extension | `str` | File extension, format is ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of `DocumentFormatConfiguration`, otherwise `None`.

### Example

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtain the singleton configuration instance
config = RedactorConfiguration.get_instance()

# Retrieve settings for the ".txt" extension
settings = config.find_format(".txt")
if settings:
    # Example: extend the list of handled extensions
    settings.extension_filter = settings.extension_filter + ",.dump"
    print("Updated extensions:", settings.extension_filter)
```

### Aliases

These names call `find_format` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `find_format_file` | `find_format_file(file_extension)` |
| `find_format_string` | `find_format_string(file_extension)` |

### See Also
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
