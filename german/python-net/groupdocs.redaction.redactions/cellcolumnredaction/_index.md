---
title: "CellColumnRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Textredaktion dar, die Text in einem Tabellendokument (CSV, Excel usw.) ersetzt."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Stellt eine Textredaktion dar, die Text in einem Tabellendokument (CSV, Excel usw.) ersetzt.

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

Der Typ CellColumnRedaction stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Initialisiert eine neue CellColumnRedaction. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und Parameter enthält. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | Der Spalten- und Arbeitsblattfilter. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Das reguläre Ausdrucksmuster zum Abgleichen. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Die [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) Instanz, die den Typ der Textersetzung angibt. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Die IOcrConnector-Implementierung, die verwendet wird, um Text aus grafischen Inhalten zu extrahieren. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
