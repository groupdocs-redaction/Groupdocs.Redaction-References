---
title: get_instance method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Returns a singleton instance with the default configuration of built-in formats."
type: docs
url: /python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Returns a singleton instance with the default configuration of built-in formats.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Example

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtain the singleton configuration
config = RedactorConfiguration.get_instance()

# Extend supported extensions for plain text formats
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### See Also
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
