---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw RedactionPolicy‑object."
type: docs
url: /nl/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuw RedactionPolicy‑object.

```python
def __init__(self):
    ...
```

### Voorbeeld

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Initialiseert een nieuw RedactionPolicy met een specifieke lijst van redacties.

```python
def __init__(self, redactions):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redactions | `list[Redaction]` | Een array van redactions voor het beleid. |

### Voorbeeld

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Zie ook
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
