---
title: "get_supported_file_types метод"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Получает поддерживаемые типы файлов."
type: docs
url: /ru/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Получает поддерживаемые типы файлов.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Пример

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Получите коллекцию поддерживаемых типов файлов
    supported_file_types = FileType.get_supported_file_types()

    # Перечислите типы файлов, отсортированные по расширению
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### См. также
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
