---
title: "метод from_extension"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Отображает расширение файла на тип файла."
type: docs
url: /ru/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Отображает расширение файла на тип файла.

```python
def from_extension(cls, extension):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| extension | `str` | Расширение файла (включая точку \".\"). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Исключения | Описание |
| :- | :- |
| `ValueError` | Когда `extension` имеет значение null или пустую строку. |

### См. также
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
