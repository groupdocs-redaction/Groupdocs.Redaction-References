---
title: "RegionReplacementOptions clase"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa los parámetros de color y área para el reemplazo de regiones de imagen."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Representa los parámetros de color y área para el reemplazo de regiones de imagen.

Más información:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

El tipo RegionReplacementOptions expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Inicializa una nueva instancia de RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Inicializa una nueva instancia de la clase RegionReplacementOptions cuyo tamaño coincide con el texto dado. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | El color utilizado para rellenar el área redactada. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | El ancho y la altura del rectángulo. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Define la posición superior‑izquierda del área a reemplazar
    point = Point(516, 311)
    # Define el tamaño del área a reemplazar
    size = Size(170, 35)
    # Utiliza un rectángulo negro sólido como reemplazo
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Guías de tareas que usan `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
