---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de RegionReplacementOptions."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Initialise une nouvelle instance de RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Couleur pour remplir la zone. |
| size | `System.Drawing.Size` | Taille de la zone remplie. |

### Exemple

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Initialise une nouvelle instance de la classe RegionReplacementOptions dont la taille correspond au texte fourni.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Couleur pour remplir la zone. |
| font | `System.Drawing.Font` | Police du texte attendu. |
| expected_text | `str` | Texte attendu. |

### Voir aussi
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
