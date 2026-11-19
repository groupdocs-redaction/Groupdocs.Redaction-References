---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a rectangle from corner coordinates and dimensions."
type: docs
url: /python-net/groupdocs.redaction.options.drawing/rectangle/__init__/
is_root: false
weight: 10
---


## __init__ {#x-y-width-height}

Initializes a rectangle from corner coordinates and dimensions.

```python
def __init__(self, x, y, width, height):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| x | `int` | Top-left horizontal offset in pixels. |
| y | `int` | Top-left vertical offset in pixels. |
| width | `int` | Area width in pixels. |
| height | `int` | Area height in pixels. |

### Example

```python
from groupdocs.redaction.options.drawing import Rectangle

# Create a rectangle at (40, 40) with width 120 and height 40
rect = Rectangle(40, 40, 120, 40)
```

## __init__ {#location-size}

Initializes a rectangle from a top-left point and region size.

```python
def __init__(self, location, size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| location | `Point` | Top-left corner of the area. |
| size | `Size` | Width and height of the area. |

### See Also
* class [`Rectangle`](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/)
