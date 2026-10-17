---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ PageAreaFilter جديدًا لتصنيف منطقة معينة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

يُنشئ PageAreaFilter جديدًا لتصنيف منطقة معينة.

```python
def __init__(self, top_left, size):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | إحداثيات المنطقة العلوية اليسرى. |
| size | `System.Drawing.Size` | حجم المنطقة واللون. |

### مثال

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### انظر أيضًا
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
