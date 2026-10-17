---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny RedactionPolicy‑instans."
type: docs
url: /sv/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny RedactionPolicy‑instans.

```python
def __init__(self):
    ...
```

### Exempel

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Initierar en ny RedactionPolicy med en specifik lista av redigeringar.

```python
def __init__(self, redactions):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| redactions | `list[Redaction]` | En array av redigeringar för policyn. |

### Exempel

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Se även
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
