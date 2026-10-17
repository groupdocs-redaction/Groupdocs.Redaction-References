---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe EraseMetadataRedaction, en effaçant toutes les métadonnées."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance de la classe EraseMetadataRedaction, en effaçant toutes les métadonnées.

```python
def __init__(self):
    ...
```

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Initialise une nouvelle instance de EraseMetadataRedaction, en effaçant les métadonnées qui correspondent aux `MetadataFilters` spécifiés.

```python
def __init__(self, filter):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| filter | `MetadataFilters` | Filtre pour les métadonnées à effacer. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Effacer toutes les métadonnées
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Effacer uniquement le champ de métadonnées auteur
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Voir aussi
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
