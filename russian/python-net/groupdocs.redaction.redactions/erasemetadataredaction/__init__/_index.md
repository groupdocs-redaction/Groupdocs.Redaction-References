---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса EraseMetadataRedaction, удаляя все метаданные."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр класса EraseMetadataRedaction, удаляя все метаданные.

```python
def __init__(self):
    ...
```

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Инициализирует новый экземпляр EraseMetadataRedaction, удаляя метаданные, соответствующие указанным `MetadataFilters`.

```python
def __init__(self, filter):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| filter | `MetadataFilters` | Фильтр для метаданных, которые нужно удалить. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Удалить все метаданные
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Удалять только поле метаданных автора
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### См. также
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
