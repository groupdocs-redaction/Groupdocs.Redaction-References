---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva AnnotationRedaction con un patrón regex y texto de reemplazo."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Inicializa una nueva AnnotationRedaction con un patrón regex y texto de reemplazo.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| pattern | `str` | Expresión regular para coincidir. |
| replacement | `str` | Reemplazo textual para el texto coincidente. |

### Ejemplo

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redactar la palabra "approved" en los textos de anotaciones
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Inicializa una nueva instancia de [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expresión regular para coincidir. |
| replacement | `str` | Reemplazo textual para el texto coincidente. |

### Ejemplo

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redactar la palabra "approved" (sin distinción de mayúsculas) y reemplazarla con "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Ver también
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
