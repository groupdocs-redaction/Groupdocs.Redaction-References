---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe PageAreaRedaction‑instantie."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Initialiseert een nieuwe PageAreaRedaction‑instantie.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |

### Voorbeeld

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

Initialiseert een nieuwe PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |
| image_options | `RegionReplacementOptions` | Vervangingsopties (afbeeldingsgebied). |

### Voorbeeld

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

### Zie ook
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
