---
title: "ImageAreaRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Redaktion dar, die ein farbiges Rechteck in einem angegebenen Bereich eines Bilddokuments platziert."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Stellt eine Redaktion dar, die ein farbiges Rechteck in einem angegebenen Bereich eines Bilddokuments platziert.

Mehr erfahren:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Der ImageAreaRedaction-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Initialisiert ein neues ImageAreaRedaction zum Redigieren eines bestimmten rechteckigen Bereichs. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und Parameter enthält. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Die RegionReplacementOptions-Optionen mit Farb- und Flächenparametern. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Die obere linke Position des zu entfernenden Bereichs. |

### Beispiel

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
Aufgabenleitfäden, die `ImageAreaRedaction` verwenden:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
