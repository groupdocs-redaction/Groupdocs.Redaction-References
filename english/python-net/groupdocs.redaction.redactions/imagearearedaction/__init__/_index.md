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
| top_left | `System.Drawing.Point` | Top-left area coordinates. |
| options | `RegionReplacementOptions` | Area size and color. |

### Example

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Define the top-left corner of the area to redact
top_left = Point(385, 485)
# Define the size and color of the redaction region
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Create the redaction object
redaction = ImageAreaRedaction(top_left, region_options)
```

### See Also
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
