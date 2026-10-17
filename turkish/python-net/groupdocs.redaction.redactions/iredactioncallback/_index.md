---
title: "IRedactionCallback sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Her bir redaksiyon değişikliği hakkında bilgi almayı sağlayan gerekli yöntemleri tanımlar ve isteğe bağlı olarak bunu önleyebilir."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Her bir redaksiyon değişikliği hakkında bilgi almayı sağlayan gerekli yöntemleri tanımlar ve isteğe bağlı olarak bunu önleyebilir.

Daha fazla bilgi:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

IRedactionCallback türü aşağıdaki üyeleri sunar:

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Belgeye herhangi bir kırpma uygulanmadan hemen önce tetiklenir, kaydetmeye veya engellemeye izin verir. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### Örnek

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

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
