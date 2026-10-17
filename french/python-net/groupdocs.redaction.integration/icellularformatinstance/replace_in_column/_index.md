---
title: "méthode replace_in_column"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Remplace toutes les correspondances par un remplacement donné dans la colonne et la feuille de calcul spécifiées."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Remplace toutes les correspondances par un remplacement donné dans la colonne et la feuille de calcul spécifiées.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| replacement | `str` | Remplacement textuel. |
| column | `int` | Indice de colonne basé sur zéro. |
| sheet | `int` | Indice de feuille de calcul basé sur zéro. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Remplace toutes les correspondances par un remplacement donné dans la colonne spécifiée sur toutes les feuilles de calcul.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| replacement | `str` | Remplacement textuel. |
| column | `int` | Indice de colonne basé sur zéro. |

**Returns:** Replacement result.

### Voir aussi
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
