---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new ImageAreaRedaction for redacting a specific rectangular area."
type: docs
url: /python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Initializes a new ImageAreaRedaction for redacting a specific rectangular area.

```python
def __init__(self, top_left, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| top_left | `Point` | Top-left area coordinates. |
| options | `RegionReplacementOptions` | Area size and color. |

### Example

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.redaction.options.drawing import Point, Size, Color

# Define the top-left corner and size of the area to redact
point = Point(385, 485)
size = Size(1793, 2069)

# Define the redaction box color
color = Color.from_argb(255, 220, 20, 60)

# Create replacement options and the redaction instance
repl_opt = RegionReplacementOptions(color, size)
img_red = ImageAreaRedaction(point, repl_opt)
```

### See Also
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
