---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny RegionReplacementOptions-instans."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Initierar en ny RegionReplacementOptions-instans.

```python
def __init__(self, fill_color, size):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Färg för att fylla området. |
| size | `System.Drawing.Size` | Storlek på fyllt område. |

### Exempel

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Initierar en ny instans av klassen RegionReplacementOptions vars storlek matchar den angivna texten.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Färg för att fylla området. |
| font | `System.Drawing.Font` | Förväntat teckensnitt för text. |
| expected_text | `str` | Förväntad text. |

### Se även
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
