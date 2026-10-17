---
title: "método initialize"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa la instancia del manejador de formato de documento."
type: docs
url: /es/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Inicializa la instancia del manejador de formato de documento.

```python
def initialize(self, config, settings):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Configuración de formato. |
| settings | `RedactorSettings` | Configuraciones predeterminadas para el proceso de redacción. |

**Returns:** None.

### Ejemplo

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

# Registrar el formato personalizado
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Ver también
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
