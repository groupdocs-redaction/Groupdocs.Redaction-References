---
title: "Класс LoadOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Предоставляет параметры, которые будут использоваться для открытия файла."
type: docs
url: /ru/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Предоставляет параметры, которые будут использоваться для открытия файла.

Узнать больше
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Тип LoadOptions раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Инициализирует новый экземпляр класса LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Инициализирует новый экземпляр LoadOptions с указанным паролем. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Инициализирует новый экземпляр LoadOptions с указанным флагом предварительной растеризации. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Инициализирует новый экземпляр LoadOptions с указанным паролем. |

### Свойства
| Свойство | Описание |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Пароль для защищённых паролем документов. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Флаг pre_rasterize, указывающий, следует ли предварительно растеризовать файл. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Укажите параметры загрузки с паролем документа
load_opt = LoadOptions("mypassword")

# Определите редактирование
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Откройте документ, защищённый паролем
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Сохраните отредактированный документ
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### См. также
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
