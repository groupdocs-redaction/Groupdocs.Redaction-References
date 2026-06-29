---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of ExactPhraseRedaction in case‑insensitive mode."
type: docs
url: /python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initializes a new instance of ExactPhraseRedaction in case‑insensitive mode.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| search_phrase | `str` | String to search and replace. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Example

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Replace occurrences of "John Doe" with "[CUSTOMER]" (case‑insensitive)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initializes a new ExactPhraseRedaction instance.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| search_phrase | `str` | String to search and replace. |
| is_case_sensitive | `bool` | True if case‑sensitive search is required. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Example

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Case‑insensitive exact phrase redaction
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Case‑sensitive exact phrase redaction
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### See Also
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
