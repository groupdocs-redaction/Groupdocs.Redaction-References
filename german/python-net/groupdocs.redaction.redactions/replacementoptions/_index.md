---
title: "ReplacementOptions Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Optionen für den Ersatz von übereinstimmendem Text dar."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Stellt Optionen für den Ersatz von übereinstimmendem Text dar.

Mehr erfahren

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Der ReplacementOptions-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Initialisiert eine neue Instanz von ReplacementOptions mit dem angegebenen Ersetzungstext. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Initialisiert eine neue Instanz der Klasse ReplacementOptions mit einem farbigen Rechteck als Option. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Die Ersetzungsaktion: Box zeichnen oder Text ersetzen. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Die Farbe für die Option `ReplacementType.draw_box` (ansonsten ignoriert). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Der benutzerdefinierte Redaktions-Handler, der es Benutzern ermöglicht, ihre eigene Redaktionslogik zu definieren. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Das Array von Filtern, das mit dieser Redaktion angewendet wird. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Der textuelle Ersetzungswert. |

### Beispiel

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ersetze übereinstimmenden Text durch den Platzhalter "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Aufgabenleitfäden, die `ReplacementOptions` verwenden:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
