---
title: "méthode initialize"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise l'instance du gestionnaire de format de document."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Initialise l'instance du gestionnaire de format de document.

```python
def initialize(self, config, settings):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Configuration du format. |
| settings | `RedactorSettings` | Paramètres par défaut pour le processus de rédaction. |

**Returns:** None.

### Exemple

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

# Enregistrer le format personnalisé
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Voir aussi
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
