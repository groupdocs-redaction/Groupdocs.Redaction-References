---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ كائن RemovePageRedaction جديد."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

ينشئ كائن RemovePageRedaction جديد.

```python
def __init__(self, origin, index, count):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| origin | `PageSeekOrigin` | ابحث عن موضع الإشارة، البداية أو النهاية لمستند. |
| index | `int` | فهرس موضع البداية (صفر‑مؤشر). |
| count | `int` | عدد الصفحات التي سيتم إزالتها. |

### مثال

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# إزالة 3 صفحات بدءًا من الصفحة الثانية (فهرس صفر‑مؤشر 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### انظر أيضًا
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
