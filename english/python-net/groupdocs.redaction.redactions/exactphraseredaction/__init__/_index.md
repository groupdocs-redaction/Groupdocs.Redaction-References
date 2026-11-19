---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of ExactPhraseRedaction class in case insensitive mode."
type: docs
url: /python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initializes a new instance of ExactPhraseRedaction class in case insensitive mode.

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

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("Emily Johnson", repl_opt)
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initializes a new ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| search_phrase | `str` | String to search and replace. |
| is_case_sensitive | `bool` | True if case‑sensitive search is required. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### See Also
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
