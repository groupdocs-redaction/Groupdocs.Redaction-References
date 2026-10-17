---
title: "Clase PageAreaFilter"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa un filtro de redacción, estableciendo un área dentro de una página de un documento para aplicar la redacción."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Representa un filtro de redacción, estableciendo un área dentro de una página de un documento para aplicar la redacción.

Aprende más

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

El tipo PageAreaFilter expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Inicializa un nuevo PageAreaFilter para redactar un área específica. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | El rectángulo (posición superior izquierda y tamaño del área) en una página. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
