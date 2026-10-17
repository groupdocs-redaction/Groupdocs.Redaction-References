---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe EraseMetadataRedaction, cancellando tutti i metadati."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza della classe EraseMetadataRedaction, cancellando tutti i metadati.

```python
def __init__(self):
    ...
```

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Inizializza una nuova istanza di EraseMetadataRedaction, cancellando i metadati che corrispondono ai `MetadataFilters` specificati.

```python
def __init__(self, filter):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| filter | `MetadataFilters` | Filtro per i metadati da cancellare. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Cancella tutti i metadati
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Cancella solo il campo metadati dell'autore
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Vedi anche
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
