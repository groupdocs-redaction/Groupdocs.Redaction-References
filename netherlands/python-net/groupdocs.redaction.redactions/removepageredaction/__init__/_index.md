---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe RemovePageRedaction."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initialiseert een nieuwe RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Zoek referentiepositie, het begin of het einde van een document. |
| index | `int` | Startpositie‑index (0‑gebaseerd). |
| count | `int` | Aantal te verwijderen pagina's. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Verwijder 3 pagina's beginnend vanaf de tweede pagina (nul‑gebaseerde index 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Zie ook
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
