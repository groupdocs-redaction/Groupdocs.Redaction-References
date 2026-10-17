---
title: "RedactorConfiguration clase"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Proporciona acceso a una lista de formatos compatibles, incluidos los incorporados y los formatos personalizados del usuario."
type: docs
url: /es/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Proporciona acceso a una lista de formatos compatibles, incluidos los incorporados y los formatos personalizados del usuario.

Más información:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

El tipo RedactorConfiguration expone los siguientes miembros:

### Métodos
| Método | Descripción |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Busca configuraciones de formato para una extensión de archivo dada. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Devuelve una instancia singleton con la configuración predeterminada de los formatos incorporados. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | La lista de formatos reconocidos, vea [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Ejemplo

```python
# Agregar un controlador de formato de usuario personalizado
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Recuperar un controlador de formato de usuario incorporado o personalizado
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Ver también
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
