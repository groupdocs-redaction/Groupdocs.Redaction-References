---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "निर्दिष्ट प्रतिस्थापन पाठ के साथ ReplacementOptions का एक नया उदाहरण प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

निर्दिष्ट प्रतिस्थापन पाठ के साथ ReplacementOptions का एक नया उदाहरण प्रारंभ करता है।

```python
def __init__(self, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| replacement | `str` | पाठ्य प्रतिस्थापन। |

### उदाहरण

```python
from groupdocs.redaction.redactions import ReplacementOptions

# मिलान किए गए टेक्स्ट को "[REDACTED]" से बदलें
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

रंगीन आयत को विकल्प के रूप में लेकर ReplacementOptions वर्ग का एक नया उदाहरण प्रारंभ करता है।

```python
def __init__(self, color):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| color | `System.Drawing.Color` | आयत का रंग। |

### संबंधित देखें
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
