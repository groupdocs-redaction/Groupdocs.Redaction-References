---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa un nuevo PageAreaFilter para redactar un área específica."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Inicializa un nuevo PageAreaFilter para redactar un área específica.

```python
def __init__(self, top_left, size):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordenadas del área superior izquierda. |
| size | `System.Drawing.Size` | Tamaño y color del área. |

### Ejemplo

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Ver también
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
