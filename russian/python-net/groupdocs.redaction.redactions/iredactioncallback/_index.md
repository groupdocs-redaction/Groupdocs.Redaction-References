---
title: "Класс IRedactionCallback"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Определяет методы, необходимые для получения информации о каждом изменении редактирования и, при необходимости, предотвращения его."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Определяет методы, необходимые для получения информации о каждом изменении редактирования и, при необходимости, предотвращения его.

Узнать больше:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Тип IRedactionCallback раскрывает следующие члены:

### Методы
| Метод | Описание |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Срабатывает непосредственно перед применением любой редактуры к документу, позволяя вести журнал или запрещать её. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
