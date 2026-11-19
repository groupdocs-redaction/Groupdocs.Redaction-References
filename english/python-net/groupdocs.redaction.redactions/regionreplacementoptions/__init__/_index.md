---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new RegionReplacementOptions instance."
type: docs
url: /python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Initializes a new RegionReplacementOptions instance.

```python
def __init__(self, fill_color, size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| fill_color | `Color` | Color to fill the area. |
| size | `Size` | Filled area size. |

### Example

```python
from groupdocs.redaction.options.drawing import Color, Size
from groupdocs.redaction.redactions import RegionReplacementOptions

color = Color.from_argb(255, 220, 20, 60)
size = Size(1793, 2069)
repl_opt = RegionReplacementOptions(color, size)
```

## __init__ {#fill_color-font-expected_text}

Initializes a new RegionReplacementOptions instance whose size matches the given text.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| fill_color | `Color` | Color to fill the area. |
| font | `Font` | Expected text font. |
| expected_text | `str` | Expected text. |

### See Also
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
