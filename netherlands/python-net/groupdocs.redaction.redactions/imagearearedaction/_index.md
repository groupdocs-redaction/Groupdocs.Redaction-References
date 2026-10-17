---
title: "ImageAreaRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een redactie voor die een gekleurde rechthoek in een opgegeven gebied van een afbeeldingsdocument plaatst."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Stelt een redactie voor die een gekleurde rechthoek in een opgegeven gebied van een afbeeldingsdocument plaatst.

Meer informatie:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Het ImageAreaRedaction type maakt de volgende leden beschikbaar:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Initialiseert een nieuwe ImageAreaRedaction voor het redigeren van een specifiek rechthoekig gebied. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | De beschrijving van de redactie, met de naam en parameters. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | De RegionReplacementOptions‑opties met kleur- en gebiedsparameters. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | De linkerbovenpositie van het te verwijderen gebied. |

### Voorbeeld

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
Taakgidsen die `ImageAreaRedaction` gebruiken:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
