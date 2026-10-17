---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue RedactionPolicy-Instanz."
type: docs
url: /de/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue RedactionPolicy-Instanz.

```python
def __init__(self):
    ...
```

### Beispiel

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Initialisiert eine neue RedactionPolicy mit einer spezifischen Liste von Redaktionen.

```python
def __init__(self, redactions):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redactions | `list[Redaction]` | Ein Array von Redaktionen für die Richtlinie. |

### Beispiel

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Siehe auch
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
