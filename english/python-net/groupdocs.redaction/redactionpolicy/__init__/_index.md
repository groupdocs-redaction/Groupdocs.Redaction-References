---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new RedactionPolicy instance."
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new RedactionPolicy instance.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Initializes a new RedactionPolicy with a specific list of redactions.

```python
def __init__(self, redactions):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redactions | `list[Redaction]` | An array of redactions for the policy. |

### Example

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### See Also
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
