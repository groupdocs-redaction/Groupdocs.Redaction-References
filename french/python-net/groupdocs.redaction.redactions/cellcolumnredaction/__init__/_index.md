---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle CellColumnRedaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Initialise une nouvelle CellColumnRedaction.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| filter | `CellFilter` | Filtre de colonne et de feuille de calcul. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement. |

### Exemple

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

### Voir aussi
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
