---
title: "Método replace_in_column"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Reemplaza todas las coincidencias con un reemplazo dado en la columna y hoja de cálculo especificadas."
type: docs
url: /es/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Reemplaza todas las coincidencias con un reemplazo dado en la columna y hoja de cálculo especificadas.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| replacement | `str` | Reemplazo textual. |
| column | `int` | Índice de columna basado en cero. |
| sheet | `int` | Índice de hoja de cálculo basado en cero. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Reemplaza todas las coincidencias con un reemplazo dado en la columna especificada en todas las hojas de cálculo.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| replacement | `str` | Reemplazo textual. |
| column | `int` | Índice de columna basado en cero. |

**Returns:** Replacement result.

### Ver también
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
