---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di ExactPhraseRedaction in modalità non sensibile al maiuscolo/minuscolo."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Inizializza una nuova istanza di ExactPhraseRedaction in modalità non sensibile al maiuscolo/minuscolo.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| search_phrase | `str` | Stringa da cercare e sostituire. |
| options | `ReplacementOptions` | Opzioni di sostituzione (testuale, colore). |

### Esempio

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Sostituisci le occorrenze di "John Doe" con "[CUSTOMER]" (non sensibile al maiuscolo/minuscolo)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Inizializza una nuova istanza di ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| search_phrase | `str` | Stringa da cercare e sostituire. |
| is_case_sensitive | `bool` | Vero se è necessaria una ricerca sensibile al maiuscolo/minuscolo. |
| options | `ReplacementOptions` | Opzioni di sostituzione (testuale, colore). |

### Esempio

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Redazione di frase esatta non sensibile al maiuscolo/minuscolo
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Redazione di frase esatta sensibile al maiuscolo/minuscolo
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Vedi anche
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
