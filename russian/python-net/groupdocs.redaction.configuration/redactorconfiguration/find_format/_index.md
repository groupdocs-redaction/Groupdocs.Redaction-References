---
title: "Метод find_format"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Находит конфигурации форматов для заданного расширения файла."
type: docs
url: /ru/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Находит конфигурации форматов для заданного расширения файла.

```python
def find_format(self, file_extension):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_extension | `str` | Расширение файла, формат — ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Пример

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Получить единственный экземпляр конфигурации
config = RedactorConfiguration.get_instance()

# Получить настройки формата для заданного расширения
settings = config.find_format(".txt")
if settings:
    # Расширить список обрабатываемых расширений, например, добавить .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### См. также
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
