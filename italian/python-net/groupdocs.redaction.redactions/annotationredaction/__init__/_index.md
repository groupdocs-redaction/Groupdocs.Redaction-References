---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova AnnotationRedaction con un modello regex e testo di sostituzione."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Inizializza una nuova AnnotationRedaction con un modello regex e testo di sostituzione.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| pattern | `str` | Espressione regolare da abbinare. |
| replacement | `str` | Sostituzione testuale per il testo corrispondente. |

### Esempio

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Oscura la parola "approved" nei testi delle annotazioni
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Inizializza una nuova istanza di [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Espressione regolare da abbinare. |
| replacement | `str` | Sostituzione testuale per il testo corrispondente. |

### Esempio

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Oscura la parola "approved" (senza distinzione tra maiuscole e minuscole) e sostituiscila con "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Vedi anche
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
