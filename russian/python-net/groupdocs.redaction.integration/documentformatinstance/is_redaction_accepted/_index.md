---
title: "метод is_redaction_accepted"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Проверяет реализацию IRedactionCallback и вызывает её, если указано."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/
is_root: false
weight: 1030
---


## is_redaction_accepted {#description}

Проверяет наличие реализации [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) и вызывает её, если указано.

```python
def is_redaction_accepted(self, description):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| description | `RedactionDescription` | Описание редактирования |

**Returns:** bool: True (by default) if redaction is accepted.

### См. также
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
