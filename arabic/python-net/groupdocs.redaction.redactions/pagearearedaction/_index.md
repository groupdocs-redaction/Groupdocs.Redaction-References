---
title: "فئة PageAreaRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل إزالة نصية معقدة تؤثر على النصوص والصور والتعليقات التوضيحية في منطقة من الصفحة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

يمثل إزالة نصية معقدة تؤثر على النصوص والصور والتعليقات التوضيحية في منطقة من الصفحة.

اعرف المزيد

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

يعرض نوع PageAreaRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | يُنشئ كائن PageAreaRedaction جديد. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | يُنشئ PageAreaRedaction جديدًا. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | يطبق Redaction على مثيل تنسيق معين. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | خيارات RegionReplacementOptions مع معلمات اللون والمساحة. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | مثيل [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) الذي يحدد نوع استبدال النص. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | وصف الإزالة، يحتوي على اسمه ومعلماته. (موروث من [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | تنفيذ IOcrConnector المستخدم لاستخراج النص من المحتوى الرسومي. (موروث من [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | نمط التعبير النمطي المستخدم للمطابقة. (موروث من [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
