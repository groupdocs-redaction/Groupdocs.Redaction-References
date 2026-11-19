---
title: apply_to method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Applies the redaction to a given format instance."
type: docs
url: /python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/
is_root: false
weight: 1010
---


## apply_to {#format_instance}

Applies the redaction to a given format instance.

Base functionality for all redactions, derived from [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) base class, is metadata filtering and it is mandatory for metadata redactions. It uses the flagged enumeration `MetadataFilters`, which contains items for the most frequent metadata entries. You can set the filter to `All` or any combination of metadata.

```python
def apply_to(self, format_instance):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| format_instance | `DocumentFormatInstance` | An instance of a document to apply redaction. |

**Returns:** Status of the redaction: success/failure and error message if any.

### Aliases

These names call `apply_to` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `apply_to_document_format_instance` | `apply_to_document_format_instance(format_instance)` |

### See Also
* class [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)
