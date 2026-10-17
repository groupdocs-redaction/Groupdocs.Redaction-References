---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de RedactionPolicy."
type: docs
url: /es/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia de RedactionPolicy.

```python
def __init__(self):
    ...
```

### Ejemplo

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Inicializa una nueva RedactionPolicy con una lista específica de redacciones.

```python
def __init__(self, redactions):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redactions | `list[Redaction]` | Una matriz de redactions para la política. |

### Ejemplo

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Ver también
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
