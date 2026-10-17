---
title: "Classe RegionReplacementOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image.

En savoir plus :
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Le type RegionReplacementOptions expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initialise une nouvelle instance de RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initialise une nouvelle instance de la classe RegionReplacementOptions dont la taille correspond au texte fourni. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | La couleur utilisée pour remplir la zone censurée. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | La largeur et la hauteur du rectangle. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Définissez la position en haut à gauche de la zone à remplacer
    point = Point(516, 311)
    # Définissez la taille de la zone à remplacer
    size = Size(170, 35)
    # Utilisez un rectangle noir plein comme remplacement
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Guides de tâches qui utilisent `RegionReplacementOptions` :

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
