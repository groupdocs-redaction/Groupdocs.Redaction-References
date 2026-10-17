---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova ImageAreaRedaction per redigere un'area rettangolare specifica."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Inizializza una nuova ImageAreaRedaction per redigere un'area rettangolare specifica.

```python
def __init__(self, top_left, options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordinate dell'area in alto a sinistra. |
| options | `RegionReplacementOptions` | Dimensione e colore dell'area. |

### Esempio

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Definisci l'angolo in alto a sinistra dell'area da oscurare
top_left = Point(385, 485)
# Definisci la dimensione e il colore della regione di oscuramento
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Crea l'oggetto di oscuramento
redaction = ImageAreaRedaction(top_left, region_options)
```

### Vedi anche
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
