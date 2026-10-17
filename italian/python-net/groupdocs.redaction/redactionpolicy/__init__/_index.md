---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di RedactionPolicy."
type: docs
url: /it/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza di RedactionPolicy.

```python
def __init__(self):
    ...
```

### Esempio

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Inizializza una nuova RedactionPolicy con un elenco specifico di redazioni.

```python
def __init__(self, redactions):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redactions | `list[Redaction]` | Un array di redactions per la policy. |

### Esempio

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Vedi anche
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
