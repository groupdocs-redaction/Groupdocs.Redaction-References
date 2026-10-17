---
title: "Clase MetadataSearchRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de metadatos que busca y redacta metadatos usando expresiones regulares, coincidiendo claves y/o valores."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Representa una redacción de metadatos que busca y redacta metadatos usando expresiones regulares, coincidiendo claves y/o valores.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

El tipo MetadataSearchRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Inicializa una nueva instancia de la clase MetadataSearchRedaction, usando el valor para coincidir con los elementos redactados. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Inicializa una nueva instancia de MetadataSearchRedaction, usando el nombre y el valor del elemento para coincidir con los elementos redactados. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Inicializa una nueva instancia de la clase MetadataSearchRedaction, usando el valor para coincidir con los elementos redactados. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Inicializa una nueva instancia de MetadataSearchRedaction usando el nombre y el valor del elemento para coincidir con los elementos redactados. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Aplica la redacción a una instancia de formato dada. (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | La descripción de la redacción, que contiene su nombre y parámetros. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | La expresión regular para coincidir con el nombre (clave) de un elemento de metadatos. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | El valor de reemplazo textual. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | La expresión regular para coincidir con el texto del valor de un elemento de metadatos. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | El filtro utilizado para seleccionar todos o metadatos específicos, como Autor o Empresa. (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Redactar cualquier valor de metadatos que coincida con el patrón
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Guías de tareas que usan `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
