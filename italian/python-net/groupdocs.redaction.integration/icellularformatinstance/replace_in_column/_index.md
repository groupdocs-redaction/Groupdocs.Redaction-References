---
title: "metodo replace_in_column"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Sostituisce tutte le corrispondenze con una data sostituzione nella colonna e nel foglio di lavoro specificati."
type: docs
url: /it/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Sostituisce tutte le corrispondenze con una data sostituzione nella colonna e nel foglio di lavoro specificati.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| replacement | `str` | Sostituzione testuale. |
| column | `int` | Indice di colonna basato su zero. |
| sheet | `int` | Indice di foglio di lavoro basato su zero. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Sostituisce tutte le corrispondenze con una data sostituzione nella colonna specificata su tutti i fogli di lavoro.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| replacement | `str` | Sostituzione testuale. |
| column | `int` | Indice di colonna basato su zero. |

**Returns:** Replacement result.

### Vedi anche
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
