---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue PageAreaRedaction-Instanz."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Initialisiert eine neue PageAreaRedaction-Instanz.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |

### Beispiel

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

Initialisiert eine neue PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |
| image_options | `RegionReplacementOptions` | Ersetzungsoptionen (Bildbereich). |

### Beispiel

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

### Siehe auch
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
