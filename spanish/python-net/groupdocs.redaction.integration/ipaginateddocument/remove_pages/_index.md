---
title: "método remove_pages"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Elimina una o varias páginas según su posición inicial, desplazamiento y cantidad."
type: docs
url: /es/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Elimina una o varias páginas según su posición inicial, desplazamiento y cantidad.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Posición de origen de búsqueda, el comienzo o el final del documento. |
| index | `int` | Índice de posición inicial (basado en 0). |
| count | `int` | Cantidad de páginas a eliminar. |

**Returns:** Pages removal redaction result.

### Ver también
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
