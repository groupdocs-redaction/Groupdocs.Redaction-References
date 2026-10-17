---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny PageAreaRedaction-instans."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Initierar en ny PageAreaRedaction-instans.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |

### Exempel

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

Initierar en ny PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |
| image_options | `RegionReplacementOptions` | Ersättningsalternativ (bildområde). |

### Exempel

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

### Se även
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
