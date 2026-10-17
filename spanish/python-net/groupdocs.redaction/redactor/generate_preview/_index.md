---
title: "Método generate_preview"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Genera imágenes de vista previa de páginas específicas en un formato de imagen dado."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Genera imágenes de vista previa de páginas específicas en un formato de imagen dado.

La vista previa se genera de acuerdo con la configuración definida en `preview_options`, que incluye el formato de imagen, dimensiones, rango de páginas y callbacks para crear y liberar flujos de página.

```python
def generate_preview(self, preview_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Propiedades de la imagen y configuraciones de rango de páginas. |

### Ejemplo

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Devuelve un flujo de archivo escribible para la imagen de vista previa de la página dada.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Se llama después de que la imagen de vista previa haya sido escrita.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Ver también
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
