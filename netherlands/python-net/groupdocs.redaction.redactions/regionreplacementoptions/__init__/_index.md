---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe RegionReplacementOptions instantie."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Initialiseert een nieuwe RegionReplacementOptions instantie.

```python
def __init__(self, fill_color, size):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Kleur om het gebied te vullen. |
| size | `System.Drawing.Size` | Gevulde gebiedsgrootte. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Initialiseert een nieuw exemplaar van de RegionReplacementOptions klasse waarvan de grootte overeenkomt met de gegeven tekst.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Kleur om het gebied te vullen. |
| font | `System.Drawing.Font` | Verwacht tekstlettertype. |
| expected_text | `str` | Verwachte tekst. |

### Zie ook
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
