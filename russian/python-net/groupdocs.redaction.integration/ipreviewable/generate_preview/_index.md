---
title: "метод generate_preview"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Создаёт предварительные изображения определённых страниц в заданном формате изображения."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Создаёт предварительные изображения определённых страниц в заданном формате изображения.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### См. также
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
