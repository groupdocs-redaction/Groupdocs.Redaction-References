---
title: "Метод get_instance"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Возвращает единственный экземпляр с конфигурацией по умолчанию встроенных форматов."
type: docs
url: /ru/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Возвращает единственный экземпляр с конфигурацией по умолчанию встроенных форматов.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Пример

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Получить единственный экземпляр конфигурации
config = RedactorConfiguration.get_instance()

# Расширить поддерживаемые расширения для форматов простого текста
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### См. также
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
