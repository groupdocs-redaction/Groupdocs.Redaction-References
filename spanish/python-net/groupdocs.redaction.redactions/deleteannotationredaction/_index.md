---
title: "Clase DeleteAnnotationRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de texto que elimina anotaciones si el texto coincide con una expresión regular dada (opcionalmente elimina todas las anotaciones)."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Representa una redacción de texto que elimina anotaciones si el texto coincide con una expresión regular dada (opcionalmente elimina todas las anotaciones).

Aprende más

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

El tipo DeleteAnnotationRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, con configuraciones para eliminar todas las anotaciones (coincidiendo con todo). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, eliminando anotaciones que coincidan con la expresión dada. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, eliminando anotaciones que coincidan con la expresión dada. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | La descripción de la redacción, que contiene el nombre de la redacción y los parámetros. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | La expresión regular a coincidir. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Eliminar anotaciones que contengan la palabra "internal" (sin distinción de mayúsculas/minúsculas)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Guías de tareas que usan `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
