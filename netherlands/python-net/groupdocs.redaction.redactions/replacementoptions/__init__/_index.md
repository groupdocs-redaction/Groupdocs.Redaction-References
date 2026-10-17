---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van ReplacementOptions met de opgegeven vervangende tekst."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Initialiseert een nieuw exemplaar van ReplacementOptions met de opgegeven vervangende tekst.

```python
def __init__(self, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| replacement | `str` | Tekstvervanging. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Vervang gevonden tekst door "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Initialiseert een nieuw exemplaar van de klasse ReplacementOptions met een gekleurde rechthoek als optie.

```python
def __init__(self, color):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| color | `System.Drawing.Color` | Rechthoekkleur. |

### Zie ook
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
