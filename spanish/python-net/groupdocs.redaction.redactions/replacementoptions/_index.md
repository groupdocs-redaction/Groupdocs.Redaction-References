---
title: "Clase ReplacementOptions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa opciones para el reemplazo de texto coincidente."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Representa opciones para el reemplazo de texto coincidente.

Aprende más

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

El tipo ReplacementOptions expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Inicializa una nueva instancia de ReplacementOptions con el texto de reemplazo especificado. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Inicializa una nueva instancia de la clase ReplacementOptions con un rectángulo coloreado como opción. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | La acción de reemplazo: dibujar cuadro o reemplazar texto. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | El color para una opción `ReplacementType.draw_box` (ignorado de lo contrario). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | El controlador de redacción personalizado que permite a los usuarios definir su propia lógica de redacción. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | La matriz de filtros a aplicar con esta redacción. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | El valor de reemplazo textual. |

### Ejemplo

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Reemplazar el texto coincidente con el marcador "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Guías de tareas que usan `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
