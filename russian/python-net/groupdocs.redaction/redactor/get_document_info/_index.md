---
title: "метод get_document_info"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Получает общую информацию о документе, такую как размер и количество страниц."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Получает общую информацию о документе, такую как размер и количество страниц.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Исключения | Описание |
| :- | :- |
| `PasswordRequiredException` | Вызывается, когда документ защищён паролем. |
| `IncorrectPasswordException` | Вызывается, когда предоставлен неверный пароль. |

### Пример

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### См. также
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
