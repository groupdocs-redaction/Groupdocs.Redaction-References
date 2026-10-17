---
title: "فئة PageAreaFilter"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل مرشح إزالة، يحدد منطقة داخل صفحة من المستند لتطبيق الإزالة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

يمثل مرشح إزالة، يحدد منطقة داخل صفحة من المستند لتطبيق الإزالة.

اعرف المزيد

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

يعرض نوع PageAreaFilter الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | يُنشئ PageAreaFilter جديدًا لتصنيف منطقة معينة. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | المستطيل (الموضع العلوي الأيسر وحجم المنطقة) في الصفحة. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
