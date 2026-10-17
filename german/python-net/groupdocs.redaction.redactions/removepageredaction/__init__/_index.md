---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue RemovePageRedaction."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initialisiert eine neue RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Referenzposition suchen, den Anfang oder das Ende eines Dokuments. |
| index | `int` | Startpositions‑Index (0‑basiert). |
| count | `int` | Anzahl der zu entfernenden Seiten. |

### Beispiel

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Entferne 3 Seiten beginnend mit der zweiten Seite (nullbasierter Index 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Siehe auch
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
