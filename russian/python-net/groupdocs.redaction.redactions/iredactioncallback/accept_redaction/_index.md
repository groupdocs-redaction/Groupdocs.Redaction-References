---
title: "метод accept_redaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Срабатывает непосредственно перед применением любой редактуры к документу, позволяя вести журнал или запрещать её."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Срабатывает непосредственно перед применением любой редактуры к документу, позволяя вести журнал или запрещать её.

```python
def accept_redaction(self, description):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| description | `RedactionDescription` | Содержит информацию о конкретном типе совпадения, критериях, тексте и позиции. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Пример

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

### См. также
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
