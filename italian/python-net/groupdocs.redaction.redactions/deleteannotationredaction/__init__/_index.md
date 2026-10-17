---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe DeleteAnnotationRedaction, con impostazioni per eliminare tutte le annotazioni (corrispondenti a tutto)."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza della classe DeleteAnnotationRedaction, con impostazioni per eliminare tutte le annotazioni (corrispondenti a tutto).

```python
def __init__(self):
    ...
```

### Esempio

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Elimina tutte le annotazioni
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita.

```python
def __init__(self, pattern):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| pattern | `str` | Espressione regolare. |

### Esempio

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Elimina le annotazioni contenenti la parola "internal" (senza distinzione tra maiuscole e minuscole)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita.

```python
def __init__(self, regex):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Espressione regolare. |

### Esempio

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Elimina le annotazioni il cui contenuto corrisponde alla regex (case‑insensitive)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Vedi anche
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
