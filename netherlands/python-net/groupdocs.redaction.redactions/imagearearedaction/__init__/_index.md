---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe ImageAreaRedaction voor het redigeren van een specifiek rechthoekig gebied."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Initialiseert een nieuwe ImageAreaRedaction voor het redigeren van een specifiek rechthoekig gebied.

```python
def __init__(self, top_left, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coördinaten van het gebied linksboven. |
| options | `RegionReplacementOptions` | Grootte en kleur van het gebied. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Definieer de linkerbovenhoek van het gebied dat moet worden geredigeerd
top_left = Point(385, 485)
# Definieer de grootte en kleur van de redactieregio
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Maak het redactobject aan
redaction = ImageAreaRedaction(top_left, region_options)
```

### Zie ook
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
