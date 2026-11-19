---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items."
type: docs
url: /python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_pattern | `str` | Regular expression to search and replace. |
| replacement | `str` | Textual replacement. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_pattern | `str` | Regular expression to search and replace metadata item value. |
| replacement | `str` | Textual replacement. |
| key_pattern | `str` | Regular expression to search and replace metadata item name. |

## __init__ {#value_regex-replacement}

Initializes a new MetadataSearchRedaction that redacts document metadata matching a regular expression.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| replacement | `str` | Textual replacement. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Redact any email address in metadata
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace metadata item value. |
| replacement | `str` | Textual replacement. |
| key_regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace metadata item name. |

### See Also
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
