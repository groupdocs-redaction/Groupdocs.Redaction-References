---
title: "فئة RegexRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل إزالة نصية تبحث وتستبدل النص في المستند عن طريق مطابقة التعبير النمطي المقدم."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

يمثل إزالة نصية تبحث وتستبدل النص في المستند عن طريق مطابقة التعبير النمطي المقدم.

اعرف المزيد

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

يعرض نوع RegexRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | ينشئ مثيلاً جديدًا من RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | ينشئ مثيلاً جديدًا من RegexRedaction. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | وصف Redaction، يحتوي على اسمه ومعاماته. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | نمط التعبير النمطي المستخدم للمطابقة. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | مثيل [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) الذي يحدد نوع استبدال النص. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | تنفيذ IOcrConnector المستخدم لاستخراج النص من المحتوى الرسومي. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # استبدال بالنص
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # استبدال بمستطيل أزرق صلب
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
أدلة المهام التي تستخدم `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
