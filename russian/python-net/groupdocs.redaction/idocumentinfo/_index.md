---
title: "Класс IDocumentInfo"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Предоставляет методы, необходимые для получения базовой информации о документе."
type: docs
url: /ru/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Предоставляет методы, необходимые для получения базовой информации о документе.

Узнайте больше: Получить информацию о файле (https://docs.groupdocs.com/redaction/net/get-file-info/).

Тип IDocumentInfo раскрывает следующие члены:

### Свойства
| Свойство | Описание |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Описание формата файла. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Общее количество страниц. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Список объектов [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/), представляющих информацию о страницах. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Размер документа в байтах. |

### Пример

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### См. также
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
