---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of EraseMetadataRedaction class, erasing all metadata."
type: docs
url: /python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of EraseMetadataRedaction class, erasing all metadata.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Initializes a new instance of EraseMetadataRedaction, erasing metadata that matches the specified `MetadataFilters`.

```python
def __init__(self, filter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filter | `MetadataFilters` | Filter for metadata to erase. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Erase all metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Erase only the author metadata field
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### See Also
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
