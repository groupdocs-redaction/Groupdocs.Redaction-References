---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva CellColumnRedaction."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Inicializa una nueva CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| filter | `CellFilter` | Filtro de columna y hoja de cálculo. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| options | `ReplacementOptions` | Opciones de reemplazo. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### Ver también
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
