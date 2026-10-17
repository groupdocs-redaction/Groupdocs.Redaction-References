---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр RedactionPolicy."
type: docs
url: /ru/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр RedactionPolicy.

```python
def __init__(self):
    ...
```

### Пример

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Инициализирует новый RedactionPolicy со специфическим списком редактирований.

```python
def __init__(self, redactions):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redactions | `list[Redaction]` | Массив редактирований для политики. |

### Пример

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### См. также
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
