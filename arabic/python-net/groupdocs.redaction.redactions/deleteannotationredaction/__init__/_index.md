---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، مع إعدادات لحذف جميع التعليقات التوضيحية (مطابقة كل شيء)."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، مع إعدادات لحذف جميع التعليقات التوضيحية (مطابقة كل شيء).

```python
def __init__(self):
    ...
```

### مثال

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# حذف جميع التعليقات التوضيحية
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، حذف التعليقات التوضيحية التي تطابق التعبير المعطى.

```python
def __init__(self, pattern):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| pattern | `str` | تعبير نمطي. |

### مثال

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# حذف التعليقات التوضيحية التي تحتوي على كلمة "internal" (غير حساسة لحالة الأحرف)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، حذف التعليقات التوضيحية التي تطابق التعبير المعطى.

```python
def __init__(self, regex):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي. |

### مثال

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# حذف التعليقات التوضيحية التي يطابق محتواها التعبير النمطي (غير حساس لحالة الأحرف)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### انظر أيضًا
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
