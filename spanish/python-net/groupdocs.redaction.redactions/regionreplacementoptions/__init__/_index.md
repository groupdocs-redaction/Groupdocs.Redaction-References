---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de RegionReplacementOptions."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Inicializa una nueva instancia de RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Color para rellenar el área. |
| size | `System.Drawing.Size` | Tamaño del área rellenada. |

### Ejemplo

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Inicializa una nueva instancia de la clase RegionReplacementOptions cuyo tamaño coincide con el texto dado.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Color para rellenar el área. |
| font | `System.Drawing.Font` | Fuente del texto esperado. |
| expected_text | `str` | Texto esperado. |

### Ver también
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
