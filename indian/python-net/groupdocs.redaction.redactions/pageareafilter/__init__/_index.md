---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "किसी विशिष्ट क्षेत्र को रिडैक्ट करने के लिए नया PageAreaFilter प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

किसी विशिष्ट क्षेत्र को रिडैक्ट करने के लिए नया PageAreaFilter प्रारंभ करता है।

```python
def __init__(self, top_left, size):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | ऊपरी-बाएँ क्षेत्र निर्देशांक. |
| size | `System.Drawing.Size` | क्षेत्र आकार और रंग. |

### उदाहरण

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### संबंधित देखें
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
