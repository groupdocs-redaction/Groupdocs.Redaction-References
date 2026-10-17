---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe LoadOptions."
type: docs
url: /it/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza della classe LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Inizializza una nuova istanza di LoadOptions con la password specificata.

```python
def __init__(self, password):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| password | `str` | Password per i file protetti. |

### Esempio

```python
    from groupdocs.redaction.options import LoadOptions

    # Carica un documento protetto da password
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Inizializza una nuova istanza di LoadOptions con il flag di pre‑rasterizzazione specificato.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| pre_rasterize | `bool` | Se True, forza la rasterizzazione al caricamento. |

## __init__ {#password-pre_rasterize}

Inizializza una nuova istanza di LoadOptions con la password specificata.

Se `pre_rasterize` è True, la rasterizzazione è forzata quando il documento viene caricato.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| password | `str` | Password per i file protetti. |
| pre_rasterize | `bool` | Se True, forza la rasterizzazione al caricamento. |

### Esempio

```python
from groupdocs.redaction.options import LoadOptions

# Carica un documento protetto da password
load_opt = LoadOptions("mypassword")
```

### Vedi anche
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
