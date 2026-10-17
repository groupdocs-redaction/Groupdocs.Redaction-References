---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр RegionReplacementOptions."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Инициализирует новый экземпляр RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Цвет для заполнения области. |
| size | `System.Drawing.Size` | Размер заполненной области. |

### Пример

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Инициализирует новый экземпляр класса RegionReplacementOptions, размер которого соответствует заданному тексту.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Цвет для заполнения области. |
| font | `System.Drawing.Font` | Ожидаемый шрифт текста. |
| expected_text | `str` | Ожидаемый текст. |

### См. также
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
