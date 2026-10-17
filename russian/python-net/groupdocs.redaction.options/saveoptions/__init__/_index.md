---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр с настройками по умолчанию: rasterizetopdf = False и addsuffix = False."
type: docs
url: /ru/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр с настройками по умолчанию: rasterize_to_pdf = False и add_suffix = False.

```python
def __init__(self):
    ...
```

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Инициализирует новый экземпляр с заданными параметрами.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, если все страницы документа необходимо преобразовать в изображения и поместить в один PDF-файл. |
| suffix | `str` | Этот текст будет добавлен в конец имени файла; если он не пустой, также устанавливает `add_suffix` в True. |

### Пример

```python
from groupdocs.redaction.options import SaveOptions

# Создать параметры сохранения с настройками по умолчанию
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### См. также
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
