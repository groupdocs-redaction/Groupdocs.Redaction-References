---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz von ReplacementOptions mit dem angegebenen Ersetzungstext."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Initialisiert eine neue Instanz von ReplacementOptions mit dem angegebenen Ersetzungstext.

```python
def __init__(self, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| replacement | `str` | Textuelle Ersetzung. |

### Beispiel

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ersetze gefundenen Text durch "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Initialisiert eine neue Instanz der Klasse ReplacementOptions mit einem farbigen Rechteck als Option.

```python
def __init__(self, color):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| color | `System.Drawing.Color` | Rechteckfarbe. |

### Siehe auch
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
