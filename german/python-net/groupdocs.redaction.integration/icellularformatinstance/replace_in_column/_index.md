---
title: "replace_in_column-Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Ersetzt alle Übereinstimmungen durch einen angegebenen Ersatz in der angegebenen Spalte und dem Arbeitsblatt."
type: docs
url: /de/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Ersetzt alle Übereinstimmungen durch einen angegebenen Ersatz in der angegebenen Spalte und dem Arbeitsblatt.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| replacement | `str` | Textuelle Ersetzung. |
| column | `int` | Nullbasierter Spaltenindex. |
| sheet | `int` | Nullbasierter Arbeitsblattindex. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Ersetzt alle Übereinstimmungen durch einen angegebenen Ersatz in der angegebenen Spalte in allen Arbeitsblättern.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| replacement | `str` | Textuelle Ersetzung. |
| column | `int` | Nullbasierter Spaltenindex. |

**Returns:** Replacement result.

### Siehe auch
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
