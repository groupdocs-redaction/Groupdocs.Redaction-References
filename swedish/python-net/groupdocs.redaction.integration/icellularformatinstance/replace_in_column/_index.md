---
title: "replace_in_column metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Ersätter alla träffar med en given ersättning i den angivna kolumnen och kalkylbladet."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Ersätter alla träffar med en given ersättning i den angivna kolumnen och kalkylbladet.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| replacement | `str` | Textuell ersättning. |
| column | `int` | Nollbaserat kolumnindex. |
| sheet | `int` | Nollbaserat arbetsbladindex. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Ersätter alla träffar med en given ersättning i den angivna kolumnen på alla kalkylblad.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| replacement | `str` | Textuell ersättning. |
| column | `int` | Nollbaserat kolumnindex. |

**Returns:** Replacement result.

### Se även
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
