---
title: "initialize Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert die Instanz des Dokumentformat-Handlers."
type: docs
url: /de/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Initialisiert die Instanz des Dokumentformat-Handlers.

```python
def initialize(self, config, settings):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Formatkonfiguration. |
| settings | `RedactorSettings` | Standardeinstellungen für den Redaktionsprozess. |

**Returns:** None.

### Beispiel

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

# Registriere das benutzerdefinierte Format
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Siehe auch
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
