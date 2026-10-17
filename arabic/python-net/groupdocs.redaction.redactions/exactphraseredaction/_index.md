---
title: "فئة ExactPhraseRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل حجبًا نصيًا يستبدل عبارة دقيقة في نص المستند، غير حساس لحالة الأحرف بشكل افتراضي."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

يمثل حجبًا نصيًا يستبدل عبارة دقيقة في نص المستند، غير حساس لحالة الأحرف بشكل افتراضي.

المزيد:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

يعرض نوع ExactPhraseRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | يقوم بتهيئة نسخة جديدة من ExactPhraseRedaction في وضع عدم حساسية الحالة. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | يقوم بتهيئة نسخة جديدة من ExactPhraseRedaction. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | وصف الحذف، يحتوي على اسم الحذف والمعلمات. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | القيمة التي تشير إلى ما إذا كان البحث حساسًا لحالة الأحرف. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | علامة اتجاه النص التي تشير إلى ما إذا كان النص من اليمين إلى اليسار. القيمة الافتراضية هي False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | السلسلة للبحث والاستبدال. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | مثيل [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) الذي يحدد نوع استبدال النص. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | تنفيذ IOcrConnector المستخدم لاستخراج النص من المحتوى الرسومي. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # استبدال حساس لحالة الأحرف
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
أدلة المهام التي تستخدم `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
