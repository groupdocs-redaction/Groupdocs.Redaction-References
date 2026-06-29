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

Learn more

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

The PageAreaRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Initializes a new PageAreaRedaction instance. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Initializes a new PageAreaRedaction. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Properties
| Property | Description |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | The RegionReplacementOptions options with color and area parameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | The [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) instance specifying the type of text replacement. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | The description of the redaction, containing its name and parameters. (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | The IOcrConnector implementation used to extract text from graphic content. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | The regular expression pattern used for matching. (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
