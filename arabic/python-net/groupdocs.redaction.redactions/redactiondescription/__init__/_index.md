---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيلاً جديدًا من فئة RedactionDescription دون معلومات استبدال."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

يُنشئ مثيلاً جديدًا من فئة RedactionDescription دون معلومات استبدال.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redaction_type | `RedactionType` | نوع البيانات التي يتم إخفاؤها. |
| action_type | `RedactionActionType` | الإجراء الذي سيُنفّذ على هذه البيانات. |
| original_text | `str` | النص المطابق أو التعليق أو محتوى التعليق التوضيحي. |

## __init__ {#redaction_type-action_type-original_text-replacement}

يُنشئ مثيلاً جديدًا من فئة RedactionDescription مع معلومات الاستبدال.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redaction_type | `RedactionType` | نوع البيانات التي يتم إخفاؤها. |
| action_type | `RedactionActionType` | الإجراء الذي سيُنفّذ على هذه البيانات. |
| original_text | `str` | النص المطابق أو التعليق أو محتوى التعليق التوضيحي. |
| replacement | `TextReplacement` | نص الاستبدال، النص المطابق وموقعه داخل السلسلة الأصلية. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

يُنشئ RedactionDescription جديدًا بمعلومات استبدال منطقة الصورة.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redaction_type | `RedactionType` | نوع البيانات التي يتم إخفاؤها. |
| action_type | `RedactionActionType` | الإجراء الذي سيُنفّذ على هذه البيانات. |
| image_area_replacement | `RegionReplacementOptions` | معلومات استبدال منطقة الصورة. |
| image_details | `str` | وصف نصي للصورة، بشكل افتراضي يكون سلسلة فارغة. |

### انظر أيضًا
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
