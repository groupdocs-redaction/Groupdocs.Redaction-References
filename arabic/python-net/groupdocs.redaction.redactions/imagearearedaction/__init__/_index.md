---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يقوم بتهيئة ImageAreaRedaction جديد لتغطية منطقة مستطيلة محددة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

يقوم بتهيئة ImageAreaRedaction جديد لتغطية منطقة مستطيلة محددة.

```python
def __init__(self, top_left, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | إحداثيات المنطقة العلوية اليسرى. |
| options | `RegionReplacementOptions` | حجم المنطقة واللون. |

### مثال

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# حدد الزاوية العليا اليسرى للمنطقة التي سيتم إخفاؤها
top_left = Point(385, 485)
# حدد الحجم واللون لمنطقة الإخفاء
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# إنشاء كائن الإخفاء
redaction = ImageAreaRedaction(top_left, region_options)
```

### انظر أيضًا
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
