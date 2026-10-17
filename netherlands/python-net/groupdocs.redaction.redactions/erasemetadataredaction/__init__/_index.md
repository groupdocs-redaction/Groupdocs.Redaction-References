---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe instantie van de EraseMetadataRedaction klasse, waarbij alle metadata worden gewist."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuwe instantie van de EraseMetadataRedaction klasse, waarbij alle metadata worden gewist.

```python
def __init__(self):
    ...
```

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Initialiseert een nieuw exemplaar van EraseMetadataRedaction, waarbij metadata wordt gewist die overeenkomt met de opgegeven `MetadataFilters`.

```python
def __init__(self, filter):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| filter | `MetadataFilters` | Filter voor metadata om te wissen. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Wis alle metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Wis alleen het auteur‑metadata‑veld.
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Zie ook
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
