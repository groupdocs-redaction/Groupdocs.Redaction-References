---
title: "Класс RedactorConfiguration"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Обеспечивает доступ к списку поддерживаемых форматов, встроенных и пользовательских."
type: docs
url: /ru/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Обеспечивает доступ к списку поддерживаемых форматов, встроенных и пользовательских.

Узнать больше:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Тип RedactorConfiguration раскрывает следующие члены:

### Методы
| Метод | Описание |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Находит конфигурации форматов для заданного расширения файла. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Возвращает единственный экземпляр с конфигурацией по умолчанию встроенных форматов. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Список распознанных форматов, см. [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Пример

```python
# Добавьте пользовательский обработчик формата
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Получите встроенный или пользовательский обработчик формата
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### См. также
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
