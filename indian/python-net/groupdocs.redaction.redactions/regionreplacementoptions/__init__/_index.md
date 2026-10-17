---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक नया RegionReplacementOptions इंस्टेंस प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

एक नया RegionReplacementOptions इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, fill_color, size):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | क्षेत्र को भरने के लिए रंग। |
| size | `System.Drawing.Size` | भरे हुए क्षेत्र का आकार। |

### उदाहरण

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

RegionReplacementOptions क्लास का एक नया इंस्टेंस प्रारंभ करता है जिसकी आकार दिया गया टेक्स्ट से मेल खाती है।

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | क्षेत्र को भरने के लिए रंग। |
| font | `System.Drawing.Font` | अपेक्षित टेक्स्ट फ़ॉन्ट। |
| expected_text | `str` | अपेक्षित टेक्स्ट। |

### संबंधित देखें
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
