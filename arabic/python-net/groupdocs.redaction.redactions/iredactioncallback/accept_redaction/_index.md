---
title: "طريقة accept_redaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يتم تشغيله مباشرةً قبل تطبيق أي إخفاء على المستند، مما يسمح بالتسجيل أو منعه."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

يتم تشغيله مباشرةً قبل تطبيق أي إخفاء على المستند، مما يسمح بالتسجيل أو منعه.

```python
def accept_redaction(self, description):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| description | `RedactionDescription` | يحتوي على معلومات حول نوع المطابقة المحدد، والمعايير، والنص، والموضع. |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
