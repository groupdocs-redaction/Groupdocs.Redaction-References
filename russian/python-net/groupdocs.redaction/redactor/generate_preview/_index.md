---
title: "метод generate_preview"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Создаёт предварительные изображения определённых страниц в заданном формате изображения."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Создаёт предварительные изображения определённых страниц в заданном формате изображения.

Предпросмотр создаётся в соответствии с настройками, определёнными в `preview_options`, которые включают формат изображения, размеры, диапазон страниц и обратные вызовы для создания и освобождения потоков страниц.

```python
def generate_preview(self, preview_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Свойства изображения и настройки диапазона страниц. |

### Пример

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Возвращает поток файла с правом записи для изображения предпросмотра данной страницы.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Вызывается после записи изображения предпросмотра.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### См. также
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
