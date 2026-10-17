---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av EraseMetadataRedaction-klass, som raderar all metadata."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny instans av EraseMetadataRedaction-klass, som raderar all metadata.

```python
def __init__(self):
    ...
```

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Initierar en ny instans av EraseMetadataRedaction, raderar metadata som matchar de angivna `MetadataFilters`.

```python
def __init__(self, filter):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| filter | `MetadataFilters` | Filter för metadata att radera. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Radera all metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Radera endast författare-metadatafältet
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Se även
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
