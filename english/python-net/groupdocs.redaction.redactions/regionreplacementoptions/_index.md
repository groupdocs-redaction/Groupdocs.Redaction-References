---
title: RegionReplacementOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents color and area parameters for image region replacement."
type: docs
url: /python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Represents color and area parameters for image region replacement.

Learn more:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

The RegionReplacementOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initializes a new RegionReplacementOptions instance. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initializes a new instance of RegionReplacementOptions class which size matches given text. |

### Properties
| Property | Description |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | The color used to fill the redacted area. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | The rectangle width and height. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Define the top‑left position of the area to replace
    point = Point(516, 311)
    # Define the size of the area to replace
    size = Size(170, 35)
    # Use a solid black rectangle as the replacement
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Task guides that use `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
