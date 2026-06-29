---
title: initialize method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes the document format handler instance."
type: docs
url: /python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Initializes the document format handler instance.

```python
def initialize(self, config, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Format configuration. |
| settings | `RedactorSettings` | Default settings for the redaction process. |

**Returns:** None.

### Example

```python
from groupdocs.redaction.integration import DocumentFormatInstance, DocumentFormatConfiguration, RedactorConfiguration

class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        super().__init__()
        self.my_property = None

    def initialize(self, config, settings=None):
        super().initialize(config, settings)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]

# Register the custom format
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### See Also
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
