---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de PageAreaRedaction."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Inicializa una nueva instancia de PageAreaRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| options | `ReplacementOptions` | Opciones de reemplazo (textual, color). |

### Ejemplo

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

Inicializa un nuevo PageAreaRedaction.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| options | `ReplacementOptions` | Opciones de reemplazo (textual, color). |
| image_options | `RegionReplacementOptions` | Opciones de reemplazo (área de imagen). |

### Ejemplo

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

### Ver también
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
