---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise un nouveau ImageAreaRedaction pour masquer une zone rectangulaire spécifique."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Initialise un nouveau ImageAreaRedaction pour masquer une zone rectangulaire spécifique.

```python
def __init__(self, top_left, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordonnées de la zone en haut à gauche. |
| options | `RegionReplacementOptions` | Taille et couleur de la zone. |

### Exemple

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Définissez le coin supérieur gauche de la zone à masquer
top_left = Point(385, 485)
# Définissez la taille et la couleur de la région de masquage
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Créez l'objet de masquage
redaction = ImageAreaRedaction(top_left, region_options)
```

### Voir aussi
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
