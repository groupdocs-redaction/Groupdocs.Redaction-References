---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de RedactionPolicy."
type: docs
url: /fr/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance de RedactionPolicy.

```python
def __init__(self):
    ...
```

### Exemple

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Initialise un nouveau RedactionPolicy avec une liste spécifique de redactions.

```python
def __init__(self, redactions):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redactions | `list[Redaction]` | Un tableau de redactions pour la politique. |

### Exemple

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Voir aussi
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
