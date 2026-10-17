---
title: "метод apply"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Применяет редактирование к документу."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Применяет редактирование к документу.

```python
def apply(self, redaction):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redaction | `Redaction` | Экземпляр `Redaction` для применения. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Пример

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Определите редактирование для замены шаблонов SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Загрузите документ и примените редактирование.
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Применяет набор редактирований к документу.

```python
def apply(self, redactions):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redactions | `list[Redaction]` | Массив редактирований для применения. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Пример

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataSearchRedaction,
    ReplacementOptions,
)
from groupdocs.redaction.metadata import MetadataFilter

redaction_list = [
    ExactPhraseRedaction("ClientName", ReplacementOptions("[client]")),
    ExactPhraseRedaction("ClientAddress", ReplacementOptions("[address]")),
    RegexRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[ssn]")),
    RegexRedaction(r"\d{16}", ReplacementOptions("[card]")),
    DeleteAnnotationRedaction(r"(?im:(use|show|describe))"),
    EraseMetadataRedaction(MetadataFilter.Author),
    MetadataSearchRedaction("CompanyName", "--company--"),
]

with Redactor("./test.docx") as redactor:
    result = redactor.apply(redaction_list)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#policy}

Применяет политику редактирования к документу.

```python
def apply(self, policy):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| policy | `RedactionPolicy` | Политика редактирования. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Пример

```python
import os
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import RasterizationOptions

policy = RedactionPolicy.load("RedactionPolicy.xml")
for file_name in os.listdir(r"C:\Inbound"):
    file_path = os.path.join(r"C:\Inbound", file_name)
    with Redactor(file_path) as redactor:
        result = redactor.apply(policy)
        out_folder = (
            r"C:\Outbound\Done"
            if result.status != RedactionStatus.FAILED
            else r"C:\Outbound\Failed"
        )
        out_path = os.path.join(out_folder, file_name)
        with open(out_path, "r+b") as stream:
            redactor.save(stream, RasterizationOptions(enabled=False))
```

### См. также
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
