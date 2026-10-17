---
title: "initialize metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar dokumentformatshanterarens instans."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Initierar dokumentformatshanterarens instans.

```python
def initialize(self, config, settings):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Formatkonfiguration. |
| settings | `RedactorSettings` | Standardinställningar för redigeringsprocessen. |

**Returns:** None.

### Exempel

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

# Registrera det anpassade formatet
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Se även
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
