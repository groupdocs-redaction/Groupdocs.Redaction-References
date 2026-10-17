---
title: "metodo initialize"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza l'istanza del gestore del formato documento."
type: docs
url: /it/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Inizializza l'istanza del gestore del formato documento.

```python
def initialize(self, config, settings):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Configurazione del formato. |
| settings | `RedactorSettings` | Impostazioni predefinite per il processo di redazione. |

**Returns:** None.

### Esempio

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

# Registra il formato personalizzato
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Vedi anche
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
