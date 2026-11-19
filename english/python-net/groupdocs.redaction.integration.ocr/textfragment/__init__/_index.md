---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a recognized text fragment."
type: docs
url: /python-net/groupdocs.redaction.integration.ocr/textfragment/__init__/
is_root: false
weight: 10
---


## __init__ {#text-rectangle}

Initializes a recognized text fragment.

```python
def __init__(self, text, rectangle):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text | `str` | textual content of the recognized text fragment. |
| rectangle | `Rectangle` | bounding rectangle of the recognized text fragment. |

### Example

```python
from groupdocs.redaction.integration.ocr import TextFragment
from groupdocs.redaction.options.drawing import Rectangle

fragment = TextFragment("Emily Johnson", Rectangle(40, 40, 230, 40))
```

### See Also
* class [`TextFragment`](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/)
