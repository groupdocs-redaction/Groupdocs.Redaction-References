---
title: "Класс Redactor"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Представляет основной класс, который контролирует процесс редактирования документов, позволяя открывать, редактировать и сохранять документы."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Представляет основной класс, который контролирует процесс редактирования документов, позволяя открывать, редактировать и сохранять документы.

Узнать больше
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Тип Redactor раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Инициализирует новый экземпляр Redactor, используя путь к файлу. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) с использованием потока. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) для защищённого паролем документа, используя его путь. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Инициализирует новый экземпляр Redactor для защищённого паролем документа, используя его путь и настройки. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Инициализирует новый экземпляр Redactor для защищённого паролем документа, используя поток. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) для защищённого паролем документа, используя поток и настройки. |

### Методы
| Метод | Описание |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Применяет редактирование к документу. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Применяет набор редактирований к документу. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Применяет политику редактирования к документу. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Освобождает ресурсы. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Создаёт предварительные изображения определённых страниц в заданном формате изображения. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Получает общую информацию о документе, такую как размер и количество страниц. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Сохраняет документ в файл со следующими параметрами: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Сохраняет документ в файл. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Сохраняет документ в поток, включая пользовательское расположение. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Откройте документ и удалите первую страницу
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Руководства задач, использующие `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### См. также
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
