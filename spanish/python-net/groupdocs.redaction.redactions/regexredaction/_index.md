---
title: "Clase RegexRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada.

Aprende más

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

El tipo RegexRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Inicializa una nueva instancia de RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Inicializa una nueva instancia de RegexRedaction. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | La descripción de la redacción, que contiene su nombre y parámetros. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | El patrón de expresión regular usado para la coincidencia. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | La instancia [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) que especifica el tipo de reemplazo de texto. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | La implementación IOcrConnector usada para extraer texto del contenido gráfico. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # reemplazar con texto
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # reemplazar con rectángulo sólido azul
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Guías de tareas que usan `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
