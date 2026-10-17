---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса RedactionDescription без информации о замене."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Инициализирует новый экземпляр класса RedactionDescription без информации о замене.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redaction_type | `RedactionType` | Тип данных, подлежащих редактированию. |
| action_type | `RedactionActionType` | Действие, которое будет выполнено над этими данными. |
| original_text | `str` | Найденный текст, комментарий или тело аннотации. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Инициализирует новый экземпляр класса RedactionDescription с информацией о замене.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redaction_type | `RedactionType` | Тип данных, подлежащих редактированию. |
| action_type | `RedactionActionType` | Действие, которое будет выполнено над этими данными. |
| original_text | `str` | Найденный текст, комментарий или тело аннотации. |
| replacement | `TextReplacement` | Текст замены, найденный текст и его позиция в оригинальной строке. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Инициализирует новый RedactionDescription с информацией о замене области изображения.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| redaction_type | `RedactionType` | Тип данных, подлежащих редактированию. |
| action_type | `RedactionActionType` | Действие, которое будет выполнено над этими данными. |
| image_area_replacement | `RegionReplacementOptions` | Информация о замене области изображения. |
| image_details | `str` | Текстовое описание изображения, по умолчанию это пустая строка. |

### См. также
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
