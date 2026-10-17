---
title: "Clase DocumentFormatInstance"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa un formato específico de un documento y puede implementarse para agregar tipos de documento personalizados."
type: docs
url: /es/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Representa un formato específico de un documento y puede implementarse para agregar tipos de documento personalizados.

Aprende más

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

El tipo DocumentFormatInstance expone los siguientes miembros:

### Métodos
| Método | Descripción |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Inicializa la instancia del manejador de formato de documento. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Verifica la implementación de [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) y la invoca, si se especifica. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Carga el documento desde un flujo. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Comprueba si el flujo dado contiene un documento compatible con esta instancia de formato. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Guarda el documento en un flujo. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | La contraseña para documentos protegidos con contraseña. |

### Ejemplo

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # cargar contenido del archivo
        pass

    def save(self, output: io.RawIOBase) -> None:
        # guardar cambios en el archivo
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### Ver también
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
