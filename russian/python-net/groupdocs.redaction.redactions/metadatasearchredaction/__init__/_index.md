---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса MetadataSearchRedaction, используя значение для сопоставления скрываемых элементов."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Инициализирует новый экземпляр класса MetadataSearchRedaction, используя значение для сопоставления скрываемых элементов.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| value_pattern | `str` | Регулярное выражение для поиска и замены |
| replacement | `str` | Текстовая замена |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Инициализирует новый экземпляр MetadataSearchRedaction, используя имя элемента и значение для сопоставления скрываемых элементов.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| value_pattern | `str` | Регулярное выражение для поиска и замены значения элемента метаданных. |
| replacement | `str` | Текстовая замена. |
| key_pattern | `str` | Регулярное выражение для поиска и замены имени элемента метаданных. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Заменить любой адрес электронной почты, найденный в значениях метаданных
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Инициализирует новый экземпляр класса MetadataSearchRedaction, используя значение для сопоставления скрываемых элементов.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| replacement | `str` | Текстовая замена. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Замаскировать любой адрес электронной почты в метаданных
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Инициализирует новый экземпляр MetadataSearchRedaction, используя имя элемента и значение для сопоставления скрываемых элементов.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены значения элемента метаданных. |
| replacement | `str` | Текстовая замена. |
| key_regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены имени элемента метаданных. |

### Пример

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Замаскировать адреса электронной почты в значениях метаданных
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### См. также
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
