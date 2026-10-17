---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva ImageAreaRedaction para redactar un área rectangular específica."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Inicializa una nueva ImageAreaRedaction para redactar un área rectangular específica.

```python
def __init__(self, top_left, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordenadas del área superior izquierda. |
| options | `RegionReplacementOptions` | Tamaño y color del área. |

### Ejemplo

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Definir la esquina superior izquierda del área a redactar
top_left = Point(385, 485)
# Definir el tamaño y color de la región de redacción
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Crear el objeto de redacción
redaction = ImageAreaRedaction(top_left, region_options)
```

### Ver también
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
