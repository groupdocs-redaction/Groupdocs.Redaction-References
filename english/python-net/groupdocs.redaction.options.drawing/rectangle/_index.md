---
title: Rectangle class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Describes a rectangular area on a page or image, for example an OCR text bounds or a redaction box."
type: docs
url: /python-net/groupdocs.redaction.options.drawing/rectangle/
is_root: false
weight: 50
---


## Rectangle class

Describes a rectangular area on a page or image, for example an OCR text bounds or a redaction box.

The Rectangle type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/__init__/#x-y-width-height) | Initializes a rectangle from corner coordinates and dimensions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/__init__/#location-size) | Initializes a rectangle from a top-left point and region size. |

### Methods
| Method | Description |
| :- | :- |
| [equals](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/equals/#other) | Compares the bounds with another rectangle. |
| [equals](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/equals/#obj) | Compares this rectangle with another object. |
| [get_hash_code](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/get_hash_code/) | Returns a hash code derived from position and size. |
| [to_string](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/to_string/) | Returns the bounds in a readable form. |

### Properties
| Property | Description |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/height/) | The height of the area, in pixels. |
| [is_empty](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/is_empty/) | The rectangle is empty. |
| [location](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/location/) | The top-left corner of the rectangle. |
| [size](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/size/) | The width and height of the rectangle. |
| [width](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/width/) | The width of the area, in pixels. |
| [x](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/x/) | The horizontal position of the top-left corner, in pixels. |
| [y](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/y/) | The vertical position of the top-left corner, in pixels. |

### Fields
| Field | Description |
| :- | :- |
| [EMPTY](/redaction/python-net/groupdocs.redaction.options.drawing/rectangle/empty/) | A rectangle with zero width and height at the origin. |

### Example

```python
from groupdocs.redaction.options.drawing import Rectangle

# Define a rectangle at position (40, 40) with size 120x40
rect = Rectangle(40, 40, 120, 40)
print(rect)
```

### Guides
Task guides that use `Rectangle`:

* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)

### See Also
* module [`groupdocs.redaction.options.drawing`](/redaction/python-net/groupdocs.redaction.options.drawing/)
