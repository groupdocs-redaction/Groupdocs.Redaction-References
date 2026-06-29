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
| value_pattern | `str` | Regular expression to search and replace |
| replacement | `str` | Textual replacement |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initializes a new instance of MetadataSearchRedaction, using item name and value to match redacted items.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_pattern | `str` | Regular expression to search and replace metadata item value. |
| replacement | `str` | Textual replacement. |
| key_pattern | `str` | Regular expression to search and replace metadata item name. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Replace any email address found in metadata values
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items.

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

Initializes a new instance of MetadataSearchRedaction using item name and value to match redacted items.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace metadata item value. |
| replacement | `str` | Textual replacement. |
| key_regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace metadata item name. |

### Example

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Redact email addresses in metadata values
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### See Also
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
