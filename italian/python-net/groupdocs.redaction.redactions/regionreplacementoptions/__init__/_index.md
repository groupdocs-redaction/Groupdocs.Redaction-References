---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di RegionReplacementOptions."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Inizializza una nuova istanza di RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Colore per riempire l'area. |
| size | `System.Drawing.Size` | Dimensione dell'area riempita. |

### Esempio

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Inizializza una nuova istanza della classe RegionReplacementOptions la cui dimensione corrisponde al testo fornito.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Colore per riempire l'area. |
| font | `System.Drawing.Font` | Carattere del testo previsto. |
| expected_text | `str` | Testo previsto. |

### Vedi anche
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
