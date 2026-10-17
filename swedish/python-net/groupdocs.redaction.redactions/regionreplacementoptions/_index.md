---
title: "RegionReplacementOptions-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar färg- och områdesparametrar för ersättning av bildregion."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Representerar färg- och områdesparametrar för ersättning av bildregion.

Läs mer:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Typen RegionReplacementOptions visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initierar en ny RegionReplacementOptions-instans. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initierar en ny instans av klassen RegionReplacementOptions vars storlek matchar den angivna texten. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Färgen som används för att fylla det redigerade området. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Rektangelns bredd och höjd. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Definiera den övre vänstra positionen för området som ska ersättas
    point = Point(516, 311)
    # Definiera storleken på området som ska ersättas
    size = Size(170, 35)
    # Använd en solid svart rektangel som ersättning
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Uppgiftsguider som använder `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
