---
title: "ReplacementOptions-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar alternativ för ersättning av matchad text."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Representerar alternativ för ersättning av matchad text.

Läs mer

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Typen ReplacementOptions exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Initierar en ny instans av ReplacementOptions med den angivna ersättningstexten. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Initierar en ny instans av klassen ReplacementOptions med färgad rektangel som ett alternativ. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Ersättningsåtgärden: rita ruta eller ersätta text. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Färgen för ett `ReplacementType.draw_box`-alternativ (ignoreras annars). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Den anpassade raderingshanteraren som låter användare definiera sin egen raderingslogik. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Arrayen med filter som ska tillämpas med denna radering. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Det textuella ersättningsvärdet. |

### Exempel

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ersätt matchad text med platshållaren "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Uppgiftsguider som använder `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
