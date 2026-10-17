---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक विशिष्ट आयताकार क्षेत्र को हटाने के लिए नया ImageAreaRedaction आरंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

एक विशिष्ट आयताकार क्षेत्र को हटाने के लिए नया ImageAreaRedaction आरंभ करता है।

```python
def __init__(self, top_left, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | ऊपरी-बाएँ क्षेत्र निर्देशांक. |
| options | `RegionReplacementOptions` | क्षेत्र आकार और रंग. |

### उदाहरण

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# रीडैक्ट करने वाले क्षेत्र के टॉप‑लेफ्ट कोने को परिभाषित करें।
top_left = Point(385, 485)
# रीडैक्शन क्षेत्र का आकार और रंग परिभाषित करें।
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# रीडैक्शन ऑब्जेक्ट बनाएं।
redaction = ImageAreaRedaction(top_left, region_options)
```

### संबंधित देखें
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
