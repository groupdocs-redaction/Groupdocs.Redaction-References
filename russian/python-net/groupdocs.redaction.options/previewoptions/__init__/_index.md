---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр PreviewOptions."
type: docs
url: /ru/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Инициализирует новый экземпляр PreviewOptions. Поток вывода будет закрыт после использования.

```python
def __init__(self, create_page_stream):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Создаёт поток для предварительного просмотра конкретной страницы. |

## __init__ {#create_page_stream-release_page_stream}

Инициализирует новый экземпляр PreviewOptions, при этом поток вывода возвращается клиенту для дальнейшего использования.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Создаёт поток для предварительного просмотра конкретной страницы. |
| release_page_stream | `ReleasePageStream` | Уведомляет, что генерация предварительного просмотра страницы завершена, и получает выходной поток. |

### См. также
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
