---
title: "Класс SaveOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Предоставляет параметры для изменения имени выходного файла и/или конвертации документа в PDF на основе изображений (растеризация)."
type: docs
url: /ru/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Предоставляет параметры для изменения имени выходного файла и/или конвертации документа в PDF на основе изображений (растеризация).

Узнать больше:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

Тип SaveOptions раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Инициализирует новый экземпляр с настройками по умолчанию: rasterize_to_pdf = False и add_suffix = False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Инициализирует новый экземпляр с заданными параметрами. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | Свойство add_suffix указывает, следует ли изменять имя файла перед сохранением. По умолчанию False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | Настройки растеризации. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | Флаг, указывающий, преобразуются ли все страницы документа в изображения и объединяются в один PDF‑файл. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Пользовательский суффикс для имени выходного файла. Если не указан, используется константа [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/). |

### Поля
| Поле | Описание |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Представляет значение суффикса по умолчанию, которое равно "Redacted". |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Сохранить документ с параметрами по умолчанию (растеризовать в PDF и добавить суффикс)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
Руководства задач, использующие `SaveOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### См. также
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
