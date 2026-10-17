---
title: "метод save"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Сохраняет документ в файл со следующими параметрами: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Сохраняет документ в файл со следующими параметрами: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Сохраняет документ в файл.

```python
def save(self, save_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| save_options | `SaveOptions` | Параметры для добавления суффикса или растеризации. |

**Returns:** Path to redacted document.

### Пример

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Укажите параметры редактирования
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        redactor.apply(ex_red)

        # Сохранить редактируемый документ в его оригинальном формате с датой в суффиксе
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Сохраняет документ в поток, включая пользовательское расположение.

```python
def save(self, document, rasterization_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| document | `io.RawIOBase` | Целевой поток. |
| rasterization_options | `RasterizationOptions` | Параметры для растеризации или её отключения и указания страниц для растеризации. |

### Пример

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # настроить растеризацию для обработки только первого слайда
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # объект BytesIO теперь содержит сохранённый документ
    data = stream.getvalue()
```

### См. также
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
