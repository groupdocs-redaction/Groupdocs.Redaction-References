---
title: "Clase ExactPhraseRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de texto que reemplaza una frase exacta en el texto del documento, sin distinción de mayúsculas por defecto."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Representa una redacción de texto que reemplaza una frase exacta en el texto del documento, sin distinción de mayúsculas por defecto.

Más información:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

El tipo ExactPhraseRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Inicializa una nueva instancia de ExactPhraseRedaction en modo sin distinción de mayúsculas y minúsculas. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Inicializa una nueva instancia de ExactPhraseRedaction. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | La descripción de la redacción, que contiene el nombre de la redacción y los parámetros. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | El valor que indica si la búsqueda distingue entre mayúsculas y minúsculas. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | La bandera de dirección del texto que indica si el texto es de derecha a izquierda. Por defecto es False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | La cadena a buscar y reemplazar. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | La instancia [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) que especifica el tipo de reemplazo de texto. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | La implementación IOcrConnector usada para extraer texto del contenido gráfico. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # reemplazo sensible a mayúsculas y minúsculas
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Guías de tareas que usan `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
