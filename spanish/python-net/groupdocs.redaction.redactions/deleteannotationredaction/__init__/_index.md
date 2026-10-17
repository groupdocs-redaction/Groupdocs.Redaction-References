---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, con configuraciones para eliminar todas las anotaciones (coincidiendo con todo)."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, con configuraciones para eliminar todas las anotaciones (coincidiendo con todo).

```python
def __init__(self):
    ...
```

### Ejemplo

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Eliminar todas las anotaciones
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, eliminando anotaciones que coincidan con la expresión dada.

```python
def __init__(self, pattern):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| pattern | `str` | Expresión regular. |

### Ejemplo

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Eliminar anotaciones que contengan la palabra "internal" (sin distinción de mayúsculas/minúsculas)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Inicializa una nueva instancia de la clase DeleteAnnotationRedaction, eliminando anotaciones que coincidan con la expresión dada.

```python
def __init__(self, regex):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expresión regular. |

### Ejemplo

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Eliminar anotaciones cuyo contenido coincide con la expresión regular (insensible a mayúsculas/minúsculas)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Ver también
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
