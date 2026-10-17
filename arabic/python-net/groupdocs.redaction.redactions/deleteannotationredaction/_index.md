---
title: "فئة DeleteAnnotationRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل حجبًا نصيًا يحذف التعليقات إذا كان النص يتطابق مع تعبير نمطي معين (يمكنه حذف جميع التعليقات اختياريًا)."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

يمثل حجبًا نصيًا يحذف التعليقات إذا كان النص يتطابق مع تعبير نمطي معين (يمكنه حذف جميع التعليقات اختياريًا).

اعرف المزيد

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

يعرض نوع DeleteAnnotationRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، مع إعدادات لحذف جميع التعليقات التوضيحية (مطابقة كل شيء). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، حذف التعليقات التوضيحية التي تطابق التعبير المعطى. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | ينشئ مثيلًا جديدًا من فئة DeleteAnnotationRedaction، حذف التعليقات التوضيحية التي تطابق التعبير المعطى. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | وصف الحذف، يحتوي على اسم الحذف والمعلمات. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | التعبير النمطي للمطابقة. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # حذف التعليقات التوضيحية التي تحتوي على كلمة "internal" (غير حساسة لحالة الأحرف)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
دلائل المهام التي تستخدم `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
