---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert ein neues ImageAreaRedaction zum Redigieren eines bestimmten rechteckigen Bereichs."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Initialisiert ein neues ImageAreaRedaction zum Redigieren eines bestimmten rechteckigen Bereichs.

```python
def __init__(self, top_left, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinaten des oberen linken Bereichs. |
| options | `RegionReplacementOptions` | Bereichsgröße und Farbe. |

### Beispiel

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Definieren Sie die obere linke Ecke des zu zensierenden Bereichs
top_left = Point(385, 485)
# Definieren Sie die Größe und Farbe des Zensurbereichs
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Erstelle das Redaktionsobjekt
redaction = ImageAreaRedaction(top_left, region_options)
```

### Siehe auch
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
