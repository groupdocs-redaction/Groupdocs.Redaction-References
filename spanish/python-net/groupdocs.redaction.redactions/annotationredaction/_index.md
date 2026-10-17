---
title: "Clase AnnotationRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción que reemplaza el texto de anotaciones (comentarios, etc.) que coinciden con una expresión regular dada."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Representa una redacción que reemplaza el texto de anotaciones (comentarios, etc.) que coinciden con una expresión regular dada.

Aprende más

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

El tipo AnnotationRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Inicializa una nueva AnnotationRedaction con un patrón regex y texto de reemplazo. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Inicializa una nueva instancia de [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | La descripción de la redacción, describiendo la redacción y sus parámetros. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | La expresión regular a coincidir. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | El reemplazo textual para el texto coincidente. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Guías de tareas que usan `AnnotationRedaction`:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
