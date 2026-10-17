---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase EraseMetadataRedaction, borrando todos los metadatos."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia de la clase EraseMetadataRedaction, borrando todos los metadatos.

```python
def __init__(self):
    ...
```

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Inicializa una nueva instancia de EraseMetadataRedaction, borrando los metadatos que coinciden con los `MetadataFilters` especificados.

```python
def __init__(self, filter):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| filter | `MetadataFilters` | Filtro para los metadatos a eliminar. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Borrar todos los metadatos
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Eliminar solo el campo de metadatos del autor
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Ver también
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
