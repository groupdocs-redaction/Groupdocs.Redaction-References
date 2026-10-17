---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُهيئ AnnotationRedaction جديدًا بنمط تعبير عادي ونص استبدال."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

يُهيئ AnnotationRedaction جديدًا بنمط تعبير عادي ونص استبدال.

```python
def __init__(self, pattern, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| pattern | `str` | تعبير نمطي للمطابقة. |
| replacement | `str` | استبدال نصي للنص المتطابق. |

### مثال

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# إخفاء الكلمة "approved" في نصوص التعليقات التوضيحية
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

يُهيئ نسخة جديدة من [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للمطابقة. |
| replacement | `str` | استبدال نصي للنص المتطابق. |

### مثال

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# إخفاء الكلمة "approved" (بدون حساسية لحالة الأحرف) واستبدالها بـ "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### انظر أيضًا
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
