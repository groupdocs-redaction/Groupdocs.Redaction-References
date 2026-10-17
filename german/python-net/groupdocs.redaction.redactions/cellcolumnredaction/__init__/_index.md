---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue CellColumnRedaction."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Initialisiert eine neue CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| filter | `CellFilter` | Spalten- und Arbeitsblattfilter. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen. |

### Beispiel

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

### Siehe auch
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
