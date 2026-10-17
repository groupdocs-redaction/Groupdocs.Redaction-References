---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de PageAreaRedaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Initialise une nouvelle instance de PageAreaRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |

### Exemple

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

Initialise un nouveau PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |
| image_options | `RegionReplacementOptions` | Options de remplacement (zone d'image). |

### Exemple

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

### Voir aussi
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
