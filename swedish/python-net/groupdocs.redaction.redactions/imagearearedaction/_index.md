---
title: "ImageAreaRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument.

Läs mer:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

ImageAreaRedaction-typen visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Initierar en ny ImageAreaRedaction för att maskera ett specifikt rektangulärt område. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Tillämpa redigeringen på en given formatinstans. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Beskrivningen av redigeringen, som innehåller dess namn och parametrar. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | RegionReplacementOptions-alternativen med färg- och områdesparametrar. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Den övre vänstra positionen för området som ska tas bort. |

### Exempel

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
Uppgiftsguider som använder `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
