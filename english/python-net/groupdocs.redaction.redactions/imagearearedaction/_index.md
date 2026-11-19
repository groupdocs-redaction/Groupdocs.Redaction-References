---
title: ImageAreaRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a redaction that places a colored rectangle in a given area of an image document."
type: docs
url: /python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Represents a redaction that places a colored rectangle in a given area of an image document.

Learn more:

- More details about applying redactions: <https://docs.groupdocs.com/redaction/python-net/redaction-basics/>
- More details about image redactions: <https://docs.groupdocs.com/redaction/python-net/image-redactions/>

The ImageAreaRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Initializes a new ImageAreaRedaction for redacting a specific rectangular area. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | The description of the redaction, containing its name and parameters. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | The RegionReplacementOptions options with color and area parameters. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | The top-left position of the area to remove. |
| [top_left_position](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left_position/) | The top-left position of the area to remove. This property is obsolete; use [`ImageAreaRedaction.TopLeft`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) instead. |

### Example

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.redaction.options.drawing import Color, Point, Size

def redact_image_area():
    # Define the top‑left position of the area to redact
    sample_point = Point(385, 485)
    # Define the size of the area which needs to be redacted
    sample_size = Size(1793, 2069)
    # Define the color of the redaction box
    color = Color.from_argb(255, 220, 20, 60)

    # Specify the redaction options
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Load the document to be redacted
    with Redactor("./sample.jpg") as redactor:
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
```

### Guides
Task guides that use `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
