---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der EraseMetadataRedaction Klasse und löscht alle Metadaten."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue Instanz der EraseMetadataRedaction Klasse und löscht alle Metadaten.

```python
def __init__(self):
    ...
```

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Initialisiert eine neue Instanz von EraseMetadataRedaction und löscht Metadaten, die den angegebenen `MetadataFilters` entsprechen.

```python
def __init__(self, filter):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| filter | `MetadataFilters` | Filter für zu löschende Metadaten. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Alle Metadaten löschen
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Nur das Autor-Metadatenfeld löschen
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Siehe auch
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
