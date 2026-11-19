---
title: PageAreaRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a complex textual redaction that affects text, images and annotations in an area of the page."
type: docs
url: /python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Represents a complex textual redaction that affects text, images and annotations in an area of the page.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/python-net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/python-net/use-page-area-redaction/)

The PageAreaRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Initializes a new PageAreaRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Initializes a new PageAreaRedaction. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | The image options specifying color and area parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | The [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) instance specifying the type of text replacement. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | The description of the redaction, containing its name and parameters. (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | The OCR connector implementation used to extract text from graphic content. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | The regular expression used for matching. (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, RegionReplacementOptions, ReplacementOptions
from groupdocs.redaction.options.drawing import Point, Size, Color

with Redactor("scan.pdf") as redactor:
    # redact text and its image rendering in a page area
    redaction = PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.black, Size(120, 20))
    )
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Task guides that use `PageAreaRedaction`:

* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
