---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلاً جديدًا من ReplacementOptions بالنص البديل المحدد."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

ينشئ مثيلاً جديدًا من ReplacementOptions بالنص البديل المحدد.

```python
def __init__(self, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| replacement | `str` | استبدال نصي. |

### مثال

```python
from groupdocs.redaction.redactions import ReplacementOptions

# استبدال النص المطابق بـ "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

ينشئ مثيلاً جديدًا من فئة ReplacementOptions مع مستطيل ملون كخيار.

```python
def __init__(self, color):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| color | `System.Drawing.Color` | لون المستطيل. |

### انظر أيضًا
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
