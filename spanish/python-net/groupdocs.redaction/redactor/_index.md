---
title: "Clase Redactor"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa la clase principal que controla el proceso de redacción de documentos, permitiendo abrir, redactar y guardar documentos."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Representa la clase principal que controla el proceso de redacción de documentos, permitiendo abrir, redactar y guardar documentos.

Aprende más
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

El tipo Redactor expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Inicializa una nueva instancia de Redactor usando una ruta de archivo. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) usando un flujo. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) para un documento protegido con contraseña usando su ruta. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Inicializa una nueva instancia de Redactor para un documento protegido con contraseña usando su ruta y configuraciones. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Inicializa una nueva instancia de Redactor para un documento protegido con contraseña usando un flujo. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) para un documento protegido con contraseña usando un flujo y configuraciones. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Aplica una redacción al documento. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Aplica un conjunto de redacciones al documento. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Aplica una política de redacción al documento. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Libera recursos. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Genera imágenes de vista previa de páginas específicas en un formato de imagen dado. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Recupera la información general del documento, como el tamaño y el número de páginas. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Guarda el documento en un archivo con las siguientes opciones: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Guarda el documento en un archivo. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Guarda el documento en un flujo, incluyendo ubicación personalizada. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Abrir un documento y eliminar la primera página
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Guías de tareas que usan `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Ver también
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
