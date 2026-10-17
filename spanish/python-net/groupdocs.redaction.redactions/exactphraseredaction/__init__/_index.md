---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de ExactPhraseRedaction en modo sin distinción de mayúsculas y minúsculas."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Inicializa una nueva instancia de ExactPhraseRedaction en modo sin distinción de mayúsculas y minúsculas.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| search_phrase | `str` | Cadena para buscar y reemplazar. |
| options | `ReplacementOptions` | Opciones de reemplazo (textual, color). |

### Ejemplo

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Reemplazar ocurrencias de "John Doe" con "[CUSTOMER]" (insensible a mayúsculas)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Inicializa una nueva instancia de ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| search_phrase | `str` | Cadena para buscar y reemplazar. |
| is_case_sensitive | `bool` | Verdadero si se requiere una búsqueda sensible a mayúsculas. |
| options | `ReplacementOptions` | Opciones de reemplazo (textual, color). |

### Ejemplo

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Redacción de frase exacta insensible a mayúsculas
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Redacción de frase exacta sensible a mayúsculas
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Ver también
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
