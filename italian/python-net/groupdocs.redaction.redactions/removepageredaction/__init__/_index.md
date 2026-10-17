---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza un nuovo RemovePageRedaction."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Inizializza un nuovo RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Cerca la posizione di riferimento, l'inizio o la fine di un documento. |
| index | `int` | Indice di posizione iniziale (basato su 0). |
| count | `int` | Numero di pagine da rimuovere. |

### Esempio

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Rimuovi 3 pagine a partire dalla seconda pagina (indice zero‑based 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Vedi anche
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
