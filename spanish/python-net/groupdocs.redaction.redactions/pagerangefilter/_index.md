---
title: "Clase PageRangeFilter"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa un filtro de redacción, estableciendo un rango de páginas dentro de un documento para aplicar la redacción."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Representa un filtro de redacción, estableciendo un rango de páginas dentro de un documento para aplicar la redacción.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

El tipo PageRangeFilter expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Inicializa una nueva RemovePageRedaction. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | El número de páginas a eliminar. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | El índice de posición inicial (basado en 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | La posición de referencia de búsqueda, ya sea el inicio o el final de un documento. |

### Ejemplo

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Define un filtro que apunta a la última página y a la anterior.
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# El filtro puede combinarse con otros filtros, p. ej., PageAreaFilter,
# y pasarse a ReplacementOptions.Filters al configurar una redacción.
```

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
