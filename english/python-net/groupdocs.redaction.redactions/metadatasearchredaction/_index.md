---
title: MetadataSearchRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values."
type: docs
url: /python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

The MetadataSearchRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Initializes a new instance of MetadataSearchRedaction, using item name and value to match redacted items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Initializes a new instance of MetadataSearchRedaction using item name and value to match redacted items. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Applies the redaction to a given format instance. (inherited from [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) |  (inherited from [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | The description of the redaction, containing its name and parameters. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | The regular expression to match the name (key) of a metadata item. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | The textual replacement value. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | The regular expression to match the value text of a metadata item. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | The filter used to select all or specific metadata, such as Author or Company. (inherited from [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Redact any metadata value matching the pattern
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Task guides that use `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
