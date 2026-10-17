---
title: "Класс DocumentFormatInstance"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет конкретный формат документа и может быть реализован для добавления пользовательских типов документов."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Представляет конкретный формат документа и может быть реализован для добавления пользовательских типов документов.

Узнать больше

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Тип DocumentFormatInstance раскрывает следующие члены:

### Методы
| Метод | Описание |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Инициализирует экземпляр обработчика формата документа. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Проверяет наличие реализации [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) и вызывает её, если указано. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Загружает документ из потока. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Проверяет, содержит ли данный поток документ, поддерживаемый этим экземпляром формата. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Сохраняет документ в поток. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Пароль для защищённых паролем документов. |

### Пример

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # загрузить содержимое файла
        pass

    def save(self, output: io.RawIOBase) -> None:
        # сохранить изменения в файл
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### См. также
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
