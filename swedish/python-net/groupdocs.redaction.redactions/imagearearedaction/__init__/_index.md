---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny ImageAreaRedaction för att maskera ett specifikt rektangulärt område."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Initierar en ny ImageAreaRedaction för att maskera ett specifikt rektangulärt område.

```python
def __init__(self, top_left, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinater för område uppe till vänster. |
| options | `RegionReplacementOptions` | Områdets storlek och färg. |

### Exempel

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Definiera det övre vänstra hörnet av området som ska rensas
top_left = Point(385, 485)
# Definiera storleken och färgen på rensningsområdet
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Skapa rensningsobjektet
redaction = ImageAreaRedaction(top_left, region_options)
```

### Se även
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
