---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक नया RemovePageRedaction इनिशियलाइज़ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

एक नया RemovePageRedaction इनिशियलाइज़ करता है।

```python
def __init__(self, origin, index, count):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| origin | `PageSeekOrigin` | संदर्भ स्थिति खोजें, दस्तावेज़ की शुरुआत या अंत। |
| index | `int` | शुरुआती स्थिति इंडेक्स (0‑आधारित)। |
| count | `int` | हटाने के लिए पृष्ठों की संख्या। |

### उदाहरण

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# दूसरे पृष्ठ (शून्य‑आधारित इंडेक्स 1) से शुरू होकर 3 पृष्ठ हटाएँ
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### संबंधित देखें
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
