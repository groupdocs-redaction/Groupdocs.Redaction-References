---
title: "Класс RedactorSettings"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет настройки редактирования, позволяющие настроить процесс редактирования."
type: docs
url: /ru/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Представляет настройки редактирования, позволяющие настроить процесс редактирования.

Узнать больше

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Тип RedactorSettings раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Инициализирует новый экземпляр класса RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Инициализирует новый экземпляр RedactorSettings с заданным экземпляром ILogger. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Инициализирует новый экземпляр класса RedactorSettings с заданным экземпляром IRedactionCallback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Инициализирует новый экземпляр RedactorSettings с указанным IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Инициализирует новый экземпляр RedactorSettings с указанным логгером и обратным вызовом. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Инициализирует новый экземпляр класса RedactorSettings с заданными экземплярами ILogger, IRedactionCallback и IOcrConnector. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Логгер, используемый для записи событий и ошибок. Должен быть экземпляром класса, реализующего [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | Экземпляр OCR‑коннектора, реализующий [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Обратный вызов редактирования, используемый для оценки каждого описания редактирования. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### См. также
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
