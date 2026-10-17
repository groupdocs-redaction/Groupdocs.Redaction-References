---
title: "Clase PreviewOptions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas."
type: docs
url: /es/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas.

La clase permite especificar el formato de vista previa, las dimensiones de la imagen, los números de página y los delegados que crean y, opcionalmente, liberan flujos para cada página generada.

El tipo PreviewOptions expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Inicializa una nueva instancia de PreviewOptions. El flujo de salida se cerrará después de su uso. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Inicializa una nueva instancia de PreviewOptions, haciendo que el flujo de salida se devuelva al cliente para su uso posterior. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | El delegado de creación del flujo de página. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | La altura de la vista previa de la página. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Los números de página para generar la vista previa. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | El formato de imagen de la vista previa. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | El delegado de finalización de la vista previa de la página. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | El ancho de la vista previa de la página. |

### Ejemplo

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Crear un archivo para la imagen de vista previa de la página dada
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Ver también
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
