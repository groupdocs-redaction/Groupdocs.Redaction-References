---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new PageAreaRedaction."
type: docs
url: /python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Initializes a new PageAreaRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

## __init__ {#regex-options-image_options}

Initializes a new PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regular expression to search and replace. |
| options | `ReplacementOptions` | Replacement options (textual, color). |
| image_options | `RegionReplacementOptions` | Replacement options (image area). |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.redaction.options.drawing import Color, Size

with Redactor("scan.pdf") as redactor:
    text_opts = ReplacementOptions("[SSN]")
    image_opts = RegionReplacementOptions(Color.black, Size(120, 20))
    redactor.apply(PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", text_opts, image_opts))
    redactor.save()
```

### See Also
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
