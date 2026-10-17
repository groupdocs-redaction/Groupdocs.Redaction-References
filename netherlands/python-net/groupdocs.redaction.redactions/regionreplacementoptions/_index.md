---
title: "RegionReplacementOptions klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt kleur‑ en gebiedsparameters voor vervanging van een afbeeldingsgebied voor."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Stelt kleur‑ en gebiedsparameters voor vervanging van een afbeeldingsgebied voor.

Meer informatie:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

De RegionReplacementOptions type bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initialiseert een nieuwe RegionReplacementOptions instantie. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initialiseert een nieuw exemplaar van de RegionReplacementOptions klasse waarvan de grootte overeenkomt met de gegeven tekst. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | De kleur die wordt gebruikt om het geredigeerde gebied te vullen. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | De breedte en hoogte van de rechthoek. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Definieer de linkerbovenpositie van het gebied dat moet worden vervangen
    point = Point(516, 311)
    # Definieer de grootte van het te vervangen gebied
    size = Size(170, 35)
    # Gebruik een solide zwarte rechthoek als vervanging
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Taakgidsen die `RegionReplacementOptions` gebruiken:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
