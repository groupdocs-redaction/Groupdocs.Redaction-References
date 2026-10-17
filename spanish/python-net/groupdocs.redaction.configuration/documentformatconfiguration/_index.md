---
title: "DocumentFormatConfiguration clase"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una referencia de tipo para la clase derivada de DocumentFormatInstance y una lista de extensiones de archivo compatibles para una detección de formato más rápida."
type: docs
url: /es/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Representa una referencia de tipo para la clase derivada de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) y una lista de extensiones de archivo compatibles para una detección de formato más rápida.

Aprende más

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

El tipo DocumentFormatConfiguration expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Inicializa una nueva instancia de DocumentFormatConfiguration. |

### Métodos
| Método | Descripción |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Comprueba si una extensión de archivo dada puede manejarse como DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | El tipo de una clase que hereda de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | La lista de extensiones de archivo delimitada por comas (por ejemplo ".pdf"), sin distinción de mayúsculas y minúsculas. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Los datos requeridos para la inicialización de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Ejemplo

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Crear una configuración de formato personalizada
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Ver también
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
