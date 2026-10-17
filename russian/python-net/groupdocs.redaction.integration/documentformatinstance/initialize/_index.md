---
title: "метод initialize"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует экземпляр обработчика формата документа."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Инициализирует экземпляр обработчика формата документа.

```python
def initialize(self, config, settings):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Конфигурация формата. |
| settings | `RedactorSettings` | Настройки по умолчанию для процесса редактирования. |

**Returns:** None.

### Пример

```python
from groupdocs.redaction.integration import DocumentFormatInstance, DocumentFormatConfiguration, RedactorConfiguration

class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        super().__init__()
        self.my_property = None

    def initialize(self, config, settings=None):
        super().initialize(config, settings)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]

# Зарегистрировать пользовательский формат
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### См. также
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
