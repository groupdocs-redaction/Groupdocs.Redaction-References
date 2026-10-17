---
title: "Clase EraseMetadataRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de metadatos que borra todos los metadatos o los metadatos que coinciden con filtros específicos de MetadataFilters del documento."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Representa una redacción de metadatos que borra todos los metadatos o los metadatos que coinciden con filtros específicos de MetadataFilters del documento.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

El tipo EraseMetadataRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Inicializa una nueva instancia de la clase EraseMetadataRedaction, borrando todos los metadatos. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Inicializa una nueva instancia de EraseMetadataRedaction, borrando los metadatos que coinciden con los `MetadataFilters` especificados. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Aplica la redacción a una instancia de formato dada. (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | La descripción de la redacción y sus parámetros. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | El filtro utilizado para seleccionar todos o metadatos específicos, como Autor o Empresa. (heredado de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Borrar todos los metadatos
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Borrar solo el campo de autor
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Guías de tareas que usan `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
