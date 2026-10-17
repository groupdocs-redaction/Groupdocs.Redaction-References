---
title: "Método generate_preview"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Genera imágenes de vista previa de páginas específicas en un formato de imagen dado."
type: docs
url: /es/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Genera imágenes de vista previa de páginas específicas en un formato de imagen dado.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Ver también
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
