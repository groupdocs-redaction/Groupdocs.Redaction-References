---
title: "Classe ImageAreaRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image.

En savoir plus :
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Le type ImageAreaRedaction expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Initialise un nouveau ImageAreaRedaction pour masquer une zone rectangulaire spécifique. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | La description de la rédaction, contenant son nom et ses paramètres. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Les options RegionReplacementOptions avec les paramètres de couleur et de zone. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | La position en haut à gauche de la zone à supprimer. |

### Exemple

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Guides de tâches qui utilisent `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
