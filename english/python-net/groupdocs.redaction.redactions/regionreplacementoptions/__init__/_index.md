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
| fill_color | `System.Drawing.Color` | Color to fill the area. |
| size | `System.Drawing.Size` | Filled area size. |

### Example

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Initializes a new instance of RegionReplacementOptions class which size matches given text.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Color to fill the area. |
| font | `System.Drawing.Font` | Expected text font. |
| expected_text | `str` | Expected text. |

### See Also
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
