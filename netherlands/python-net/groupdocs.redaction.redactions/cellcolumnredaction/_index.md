---
title: "CellColumnRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een tekstredactie voor die tekst vervangt in een spreadsheetdocument (CSV, Excel, enz.)."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Stelt een tekstredactie voor die tekst vervangt in een spreadsheetdocument (CSV, Excel, enz.).

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

Het type CellColumnRedaction biedt de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Initialiseert een nieuwe CellColumnRedaction. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | De beschrijving van de redactie, met de naam en parameters. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | De kolom- en werkbladfilter. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Het reguliere expressiepatroon om te matchen. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | De [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)‑instantie die het type tekstvervanging specificeert. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | De IOcrConnector‑implementatie die wordt gebruikt om tekst uit grafische inhoud te extraheren. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
