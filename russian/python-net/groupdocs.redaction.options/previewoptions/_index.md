---
title: "Класс PreviewOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра."
type: docs
url: /ru/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра.

Класс позволяет задавать формат предварительного просмотра, размеры изображения, номера страниц и делегаты, которые создают и при необходимости освобождают потоки для каждой сгенерированной страницы.

Тип PreviewOptions предоставляет следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Инициализирует новый экземпляр PreviewOptions. Поток вывода будет закрыт после использования. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Инициализирует новый экземпляр PreviewOptions, при этом поток вывода возвращается клиенту для дальнейшего использования. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Делегат создания потока страницы. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Высота предварительного просмотра страницы. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Номера страниц для генерации предварительного просмотра. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Формат изображения предварительного просмотра. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Делегат завершения предварительного просмотра страницы. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Ширина предварительного просмотра страницы. |

### Пример

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Создать файл изображения предварительного просмотра указанной страницы
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### См. также
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
