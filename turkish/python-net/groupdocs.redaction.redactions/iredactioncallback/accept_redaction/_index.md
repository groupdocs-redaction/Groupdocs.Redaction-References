---
title: "accept_redaction yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgeye herhangi bir kırpma uygulanmadan hemen önce tetiklenir, kaydetmeye veya engellemeye izin verir."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Belgeye herhangi bir kırpma uygulanmadan hemen önce tetiklenir, kaydetmeye veya engellemeye izin verir.

```python
def accept_redaction(self, description):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| description | `RedactionDescription` | Belirli eşleşme türü, kriter, metin ve konum hakkında bilgi içerir. |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
