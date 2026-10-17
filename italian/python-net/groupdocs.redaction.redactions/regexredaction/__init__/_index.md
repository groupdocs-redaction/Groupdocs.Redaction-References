---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di RegexRedaction."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Inizializza una nuova istanza di RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| pattern | `str` | Espressione regolare da cercare e sostituire. |
| options | `ReplacementOptions` | Opzioni di sostituzione (testuale, colore). |

### Esempio

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Inizializza una nuova istanza di RegexRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| options | `ReplacementOptions` | Opzioni di sostituzione (testuale, colore). |

### Esempio

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Vedi anche
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
