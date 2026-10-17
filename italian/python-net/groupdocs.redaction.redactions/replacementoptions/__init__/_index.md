---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di ReplacementOptions con il testo di sostituzione specificato."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Inizializza una nuova istanza di ReplacementOptions con il testo di sostituzione specificato.

```python
def __init__(self, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| replacement | `str` | Sostituzione testuale. |

### Esempio

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Sostituisci il testo corrispondente con "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Inizializza una nuova istanza della classe ReplacementOptions con un rettangolo colorato come opzione.

```python
def __init__(self, color):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| color | `System.Drawing.Color` | Colore del rettangolo. |

### Vedi anche
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
