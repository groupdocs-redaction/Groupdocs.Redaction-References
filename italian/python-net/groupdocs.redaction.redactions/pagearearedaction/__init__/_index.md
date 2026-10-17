---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di PageAreaRedaction."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Inizializza una nuova istanza di PageAreaRedaction.

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
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

Inizializza un nuovo PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| options | `ReplacementOptions` | Opzioni di sostituzione (testuale, colore). |
| image_options | `RegionReplacementOptions` | Opzioni di sostituzione (area immagine). |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### Vedi anche
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
