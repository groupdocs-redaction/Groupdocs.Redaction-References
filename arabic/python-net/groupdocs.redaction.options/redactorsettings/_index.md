---
title: "فئة RedactorSettings"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل إعدادات الإخفاء، مما يسمح بتخصيص عملية الإخفاء."
type: docs
url: /ar/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

يمثل إعدادات الإخفاء، مما يسمح بتخصيص عملية الإخفاء.

اعرف المزيد

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

نوع RedactorSettings يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | يُنشئ مثيلًا جديدًا لفئة RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام مثيل ILogger معين. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | يُنشئ مثيلًا جديدًا لفئة RedactorSettings باستخدام مثيل IRedactionCallback معين. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام IOcrConnector المحدد. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام logger المحدد والرد الندائي. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | يُنشئ مثيلًا جديدًا لفئة RedactorSettings باستخدام مثيلات ILogger و IRedactionCallback و IOcrConnector المعطاة. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | المُسجِل المستخدم لتسجيل الأحداث والأخطاء. يجب أن يكون مثيلًا لفئة تُنفّذ [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | مثيل موصل OCR الذي يُنفّذ [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | دالة رد النداء للتمويه المستخدمة لتقييم كل وصف للتمويه. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### انظر أيضًا
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
