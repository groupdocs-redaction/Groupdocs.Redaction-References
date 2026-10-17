---
title: "RegionReplacementOptions Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Farb- und Bereichsparameter für den Austausch von Bildregionen dar."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Stellt Farb- und Bereichsparameter für den Austausch von Bildregionen dar.

Mehr erfahren:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Der RegionReplacementOptions-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initialisiert eine neue RegionReplacementOptions-Instanz. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initialisiert eine neue Instanz der RegionReplacementOptions-Klasse, deren Größe dem angegebenen Text entspricht. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Die Farbe, die zum Füllen des geschwärzten Bereichs verwendet wird. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Die Breite und Höhe des Rechtecks. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Definieren Sie die obere‑linke Position des zu ersetzenden Bereichs
    point = Point(516, 311)
    # Definieren Sie die Größe des zu ersetzenden Bereichs
    size = Size(170, 35)
    # Verwenden Sie ein einfarbiges schwarzes Rechteck als Ersatz
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Aufgabenleitfäden, die `RegionReplacementOptions` verwenden:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
