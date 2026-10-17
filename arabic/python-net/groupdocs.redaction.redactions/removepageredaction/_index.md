---
title: "فئة RemovePageRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل إزالة تزيل صفحة (شريحة، ورقة عمل، إلخ) من المستند."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

يمثل إزالة تزيل صفحة (شريحة، ورقة عمل، إلخ) من المستند.

اعرف المزيد
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

يعرض نوع RemovePageRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | ينشئ كائن RemovePageRedaction جديد. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | عدد الصفحات التي سيتم إزالتها. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | فهرس موضع البداية (بدءًا من 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | موضع الإشارة للبحث، إما بداية المستند أو نهايته. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | وصف الحذف، يحتوي على اسمه ومعاماته. (موروث من [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # إزالة صفحة واحدة محسوبة من نهاية المستند
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # تطبيق الحجب
        result = redactor.apply(rem_opt)

        # احفظ المستند المحذوف
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
دليل المهام الذي يستخدم `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
