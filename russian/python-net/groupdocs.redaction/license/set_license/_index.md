---
title: "метод set_license"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Примените лицензию к текущему процессу."
type: docs
url: /ru/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

Примените лицензию к текущему процессу.

```python
def set_license(self, license_source):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| license_source |  | Либо строковый путь к файлу ``.lic`` либо читаемый объект, похожий на файл, который возвращает байты лицензии. Такие входные данные записываются во временный файл перед передачей в мост. |

| Исключения | Описание |
| :- | :- |
| `TypeError` | Если ``license_source`` не является ни строковым путем, ни читаемым объектом, похожим на файл. |

### См. также
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
