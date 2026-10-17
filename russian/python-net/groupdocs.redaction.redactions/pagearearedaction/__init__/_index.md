---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр PageAreaRedaction."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Инициализирует новый экземпляр PageAreaRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| options | `ReplacementOptions` | Replacement options (textual, color). |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

Инициализирует новый PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Регулярное выражение для поиска и замены. |
| options | `ReplacementOptions` | Replacement options (textual, color). |
| image_options | `RegionReplacementOptions` | Параметры замены (область изображения). |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### См. также
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
