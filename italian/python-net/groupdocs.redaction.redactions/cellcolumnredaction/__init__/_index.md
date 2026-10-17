---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova CellColumnRedaction."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Inizializza una nuova CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| filter | `CellFilter` | Filtro di colonna e foglio di lavoro. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| options | `ReplacementOptions` | Opzioni di sostituzione. |

### Esempio

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

### Vedi anche
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
