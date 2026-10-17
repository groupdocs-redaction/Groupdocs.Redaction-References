---
title: "Класс DocumentFormatConfiguration"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет ссылку на тип класса, производного от DocumentFormatInstance, и список поддерживаемых расширений файлов для более быстрого определения формата."
type: docs
url: /ru/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Представляет ссылку на тип для класса, полученного от [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/), и список поддерживаемых расширений файлов для более быстрой детекции формата.

Узнать больше

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Тип DocumentFormatConfiguration раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Инициализирует новый экземпляр DocumentFormatConfiguration. |

### Методы
| Метод | Описание |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Проверяет, может ли указанное расширение файла обрабатываться как DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Тип класса, наследующегося от [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Список расширений файлов, разделённых запятыми (например ".pdf"), без учёта регистра. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Данные, необходимые для инициализации [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Пример

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Создать пользовательскую конфигурацию формата
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### См. также
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
