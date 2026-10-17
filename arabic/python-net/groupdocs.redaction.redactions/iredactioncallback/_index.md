---
title: "فئة IRedactionCallback"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يحدد الأساليب المطلوبة لتلقي المعلومات حول كل تغيير في الإزالة وإمكانية منعها اختياريًا."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

يحدد الأساليب المطلوبة لتلقي المعلومات حول كل تغيير في الإزالة وإمكانية منعها اختياريًا.

المزيد:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

يعرض نوع IRedactionCallback الأعضاء التالية:

### الطرق
| طريقة | الوصف |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | يتم تشغيله مباشرةً قبل تطبيق أي إخفاء على المستند، مما يسمح بالتسجيل أو منعه. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
