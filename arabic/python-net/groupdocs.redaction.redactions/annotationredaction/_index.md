---
title: "فئة AnnotationRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل حجبًا يستبدل نص التعليقات (التعليقات، إلخ) المتطابق مع تعبير نمطي معين."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

يمثل حجبًا يستبدل نص التعليقات (التعليقات، إلخ) المتطابق مع تعبير نمطي معين.

اعرف المزيد

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

نوع AnnotationRedaction يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | يُهيئ AnnotationRedaction جديدًا بنمط تعبير عادي ونص استبدال. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | يُهيئ نسخة جديدة من [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | وصف الإزالة، يصف الإزالة ومعلماتها. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | التعبير النمطي للمطابقة. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | الاستبدال النصي للنص المتطابق. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
أدلة المهام التي تستخدم `AnnotationRedaction`:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
