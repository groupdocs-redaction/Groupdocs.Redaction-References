---
title: "Clase ImageAreaRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción que coloca un rectángulo coloreado en un área determinada de un documento de imagen."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Representa una redacción que coloca un rectángulo coloreado en un área determinada de un documento de imagen.

Más información:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

El tipo ImageAreaRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Inicializa una nueva ImageAreaRedaction para redactar un área rectangular específica. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | La descripción de la redacción, que contiene su nombre y parámetros. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Las opciones RegionReplacementOptions con parámetros de color y área. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | La posición superior izquierda del área a eliminar. |

### Ejemplo

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Guías de tareas que usan `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
