---
title: "Clase RemovePageRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción que elimina una página (diapositiva, hoja de cálculo, etc.) de un documento."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Representa una redacción que elimina una página (diapositiva, hoja de cálculo, etc.) de un documento.

Aprende más
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

El tipo RemovePageRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Inicializa una nueva RemovePageRedaction. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | El número de páginas a eliminar. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | El índice de posición inicial (basado en 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | La posición de referencia de búsqueda, ya sea el inicio o el final de un documento. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | La descripción de la redacción, que contiene su nombre y parámetros. (heredado de [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Eliminar 1 página contando desde el final del documento
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Aplicar la redacción
        result = redactor.apply(rem_opt)

        # Guarde el documento redactado
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Guías de tareas que usan `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
