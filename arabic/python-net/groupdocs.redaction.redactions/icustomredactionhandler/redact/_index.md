---
title: "طريقة redact"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يطبق إخفاءً مخصصاً على محتوى مستند محدد."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

يطبق إخفاءً مخصصاً على محتوى مستند محدد.

حاليًا، هذا مدعوم فقط لتنسيق PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

يمكن للمستخدمين تعريف منطق الحذف الخاص بهم، مثل الحذف المعتمد على الذكاء الاصطناعي، والذي قد يكون أكثر تقدمًا من الأساليب البسيطة القائمة على الأنماط.

```python
def redact(self, context):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| context | `CustomRedactionContext` | يحتوي على محتوى المستند الذي سيتم حذفه مع البيانات الوصفية ذات الصلة. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### انظر أيضًا
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
