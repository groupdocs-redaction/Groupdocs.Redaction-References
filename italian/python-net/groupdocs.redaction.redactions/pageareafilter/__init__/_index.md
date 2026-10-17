---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza un nuovo PageAreaFilter per redigere un'area specifica."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Inizializza un nuovo PageAreaFilter per redigere un'area specifica.

```python
def __init__(self, top_left, size):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordinate dell'area in alto a sinistra. |
| size | `System.Drawing.Size` | Dimensione e colore dell'area. |

### Esempio

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Vedi anche
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
