---
title: "فئة RedactionPolicy"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل سياسة تنقية، تحتوي على مجموعة من عمليات الإخفاء المحددة للتطبيق."
type: docs
url: /ar/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

يمثل سياسة تنقية، تحتوي على مجموعة من عمليات الإخفاء المحددة للتطبيق.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

نوع RedactionPolicy يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | ينشئ مثيلًا جديدًا من RedactionPolicy. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | ينشئ RedactionPolicy جديدًا بقائمة محددة من عمليات الحجب. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | يقوم بتحميل RedactionPolicy من ملف XML. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | يقوم بتحميل مثيل RedactionPolicy من تدفق يحتوي على تكوين XML. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | يحفظ سياسة الحجب إلى ملف. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | يحفظ سياسة الحجب إلى تدفق. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | قائمة الفئات المستمدة من [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/) والمُكوَّنة بالكامل. |

### مثال

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# بناء سياسة قابلة لإعادة الاستخدام في الذاكرة
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# تطبيق السياسة على مستند
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
أدلة المهام التي تستخدم `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
