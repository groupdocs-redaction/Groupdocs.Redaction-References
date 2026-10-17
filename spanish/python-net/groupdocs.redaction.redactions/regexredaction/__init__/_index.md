---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de RegexRedaction."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Inicializa una nueva instancia de RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| pattern | `str` | Expresión regular para buscar y reemplazar. |
| options | `ReplacementOptions` | Opciones de reemplazo (textual, color). |

### Ejemplo

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Inicializa una nueva instancia de RegexRedaction.

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
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Ver también
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
