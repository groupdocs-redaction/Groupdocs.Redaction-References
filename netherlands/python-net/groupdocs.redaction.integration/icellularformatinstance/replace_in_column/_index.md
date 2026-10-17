---
title: "replace_in_column‑methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Vervangt alle overeenkomsten met een opgegeven vervanging in de gespecificeerde kolom en werkblad."
type: docs
url: /nl/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Vervangt alle overeenkomsten met een opgegeven vervanging in de gespecificeerde kolom en werkblad.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| replacement | `str` | Tekstvervanging. |
| column | `int` | Nulgebaseerde kolomindex. |
| sheet | `int` | Nulgebaseerde werkbladindex. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Vervangt alle overeenkomsten met een opgegeven vervanging in de gespecificeerde kolom op alle werkbladen.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| replacement | `str` | Tekstvervanging. |
| column | `int` | Nulgebaseerde kolomindex. |

**Returns:** Replacement result.

### Zie ook
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
