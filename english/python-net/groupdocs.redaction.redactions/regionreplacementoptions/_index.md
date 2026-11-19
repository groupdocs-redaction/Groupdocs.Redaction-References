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

- More details about image redactions: https://docs.groupdocs.com/redaction/python-net/image-redactions/

The RegionReplacementOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Initializes a new RegionReplacementOptions instance. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Initializes a new RegionReplacementOptions instance whose size matches the given text. |

### Properties
| Property | Description |
| :- | :- |
| [area_fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/area_fill_color/) | The color used to fill the redacted area. This property is obsolete; use [`RegionReplacementOptions.FillColor`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) instead. |
| [area_size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/area_size/) | The rectangle width and height; this property is obsolete—use [`RegionReplacementOptions.size`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) instead. |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | The color used to fill the redacted area. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | The rectangle width and height. |

### Example

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.redaction.options.drawing import Color, Point, Size
from groupdocs.redaction import Redactor, RedactionStatus

def redact_image_area():
    point = Point(516, 311)
    size = Size(170, 35)
    repl_opt = RegionReplacementOptions(Color.Blue, size)
    img_red = ImageAreaRedaction(point, repl_opt)

    with Redactor("D:\\test.jpg") as redactor:
        result = redactor.apply(img_red)
        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

### Guides
Task guides that use `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
