---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يقوم بتهيئة نسخة جديدة من ExactPhraseRedaction في وضع عدم حساسية الحالة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

يقوم بتهيئة نسخة جديدة من ExactPhraseRedaction في وضع عدم حساسية الحالة.

```python
def __init__(self, search_phrase, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| search_phrase | `str` | سلسلة للبحث والاستبدال. |
| options | `ReplacementOptions` | خيارات الاستبدال (نصية، لون). |

### مثال

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# استبدال تكرارات "John Doe" بـ "[CUSTOMER]" (بدون حساسية لحالة الأحرف)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

يقوم بتهيئة نسخة جديدة من ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| search_phrase | `str` | سلسلة للبحث والاستبدال. |
| is_case_sensitive | `bool` | صحيح إذا كان البحث حساسًا لحالة الأحرف مطلوبًا. |
| options | `ReplacementOptions` | خيارات الاستبدال (نصية، لون). |

### مثال

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# إخفاء العبارة الدقيقة غير حساس لحالة الأحرف
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# إخفاء العبارة الدقيقة حساس لحالة الأحرف
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### انظر أيضًا
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
