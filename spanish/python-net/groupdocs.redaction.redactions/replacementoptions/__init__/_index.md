---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de ReplacementOptions con el texto de reemplazo especificado."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Inicializa una nueva instancia de ReplacementOptions con el texto de reemplazo especificado.

```python
def __init__(self, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| replacement | `str` | Reemplazo textual. |

### Ejemplo

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Reemplazar el texto coincidente con "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Inicializa una nueva instancia de la clase ReplacementOptions con un rectángulo coloreado como opción.

```python
def __init__(self, color):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| color | `System.Drawing.Color` | Color del rectángulo. |

### Ver también
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
