---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av ReplacementOptions med den angivna ersättningstexten."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Initierar en ny instans av ReplacementOptions med den angivna ersättningstexten.

```python
def __init__(self, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| replacement | `str` | Textuell ersättning. |

### Exempel

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ersätt matchad text med "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Initierar en ny instans av klassen ReplacementOptions med färgad rektangel som ett alternativ.

```python
def __init__(self, color):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| color | `System.Drawing.Color` | Rektangel färg. |

### Se även
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
