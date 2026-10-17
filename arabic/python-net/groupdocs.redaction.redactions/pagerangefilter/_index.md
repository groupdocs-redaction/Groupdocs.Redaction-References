---
title: "الفئة PageRangeFilter"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل مرشح إزالة، يحدد نطاق الصفحات داخل المستند لتطبيق الإزالة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

يمثل مرشح إزالة، يحدد نطاق الصفحات داخل المستند لتطبيق الإزالة.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

يعرض نوع PageRangeFilter الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | ينشئ كائن RemovePageRedaction جديد. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | عدد الصفحات التي سيتم إزالتها. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | فهرس موضع البداية (بدءًا من 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | موضع الإشارة للبحث، إما بداية المستند أو نهايته. |

### مثال

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# حدد مرشحًا يستهدف الصفحة الأخيرة والسابقة لها
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# يمكن دمج المرشح مع مرشحات أخرى، مثل PageAreaFilter،
# وتمريره إلى ReplacementOptions.Filters عند تكوين حذف.
```

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
