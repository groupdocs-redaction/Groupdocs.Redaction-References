---
title: "метод redact"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Применяет пользовательскую редактуру к определённому содержимому документа."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Применяет пользовательскую редактуру к определённому содержимому документа.

В настоящее время это поддерживается только для PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Пользователи могут определить собственную логику редактирования, например основанную на ИИ, которая может быть более продвинутой, чем простые методы, основанные на шаблонах.

```python
def redact(self, context):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| context | `CustomRedactionContext` | Содержит содержимое документа, подлежащее редактированию, вместе с сопутствующими метаданными. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### См. также
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
