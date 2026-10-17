---
title: "Classe CellColumnRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione testuale che sostituisce il testo in un documento di foglio di calcolo (CSV, Excel, ecc.)."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Rappresenta una redazione testuale che sostituisce il testo in un documento di foglio di calcolo (CSV, Excel, ecc.).

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

Il tipo CellColumnRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Inizializza una nuova CellColumnRedaction. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Applica la redazione a una data istanza di formato. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | La descrizione della redazione, contenente il suo nome e i parametri. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | Il filtro di colonna e foglio di lavoro. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Il modello di espressione regolare da corrispondere. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | L'istanza [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) che specifica il tipo di sostituzione del testo. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | L'implementazione IOcrConnector utilizzata per estrarre il testo dal contenuto grafico. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Esempio

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

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
