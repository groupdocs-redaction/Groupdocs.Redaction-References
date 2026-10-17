---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue RegionReplacementOptions-Instanz."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Initialisiert eine neue RegionReplacementOptions-Instanz.

```python
def __init__(self, fill_color, size):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Farbe zum Füllen des Bereichs. |
| size | `System.Drawing.Size` | Größe des gefüllten Bereichs. |

### Beispiel

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Initialisiert eine neue Instanz der RegionReplacementOptions-Klasse, deren Größe dem angegebenen Text entspricht.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Farbe zum Füllen des Bereichs. |
| font | `System.Drawing.Font` | Erwartete Textschriftart. |
| expected_text | `str` | Erwarteter Text. |

### Siehe auch
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
