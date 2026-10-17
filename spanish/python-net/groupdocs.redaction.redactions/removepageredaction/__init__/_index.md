---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva RemovePageRedaction."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Inicializa una nueva RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Buscar posición de referencia, el inicio o el final de un documento. |
| index | `int` | Índice de posición inicial (basado en 0). |
| count | `int` | Cantidad de páginas a eliminar. |

### Ejemplo

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Eliminar 3 páginas a partir de la segunda página (índice basado en cero 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Ver también
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
