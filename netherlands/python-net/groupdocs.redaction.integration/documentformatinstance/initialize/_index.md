---
title: "initialize methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert het exemplaar van de documentformaat-handler."
type: docs
url: /nl/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Initialiseert het exemplaar van de documentformaat-handler.

```python
def initialize(self, config, settings):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Formaatconfiguratie. |
| settings | `RedactorSettings` | Standaardinstellingen voor het redactieproces. |

**Returns:** None.

### Voorbeeld

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

# Registreer het aangepaste formaat
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Zie ook
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
