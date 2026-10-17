---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase MetadataSearchRedaction, usando el valor para coincidir con los elementos redactados."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Inicializa una nueva instancia de la clase MetadataSearchRedaction, usando el valor para coincidir con los elementos redactados.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| value_pattern | `str` | Expresión regular para buscar y reemplazar |
| replacement | `str` | Reemplazo textual |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Inicializa una nueva instancia de MetadataSearchRedaction, usando el nombre y el valor del elemento para coincidir con los elementos redactados.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| value_pattern | `str` | Expresión regular para buscar y reemplazar el valor del elemento de metadatos. |
| replacement | `str` | Reemplazo textual. |
| key_pattern | `str` | Expresión regular para buscar y reemplazar el nombre del elemento de metadatos. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Reemplazar cualquier dirección de correo electrónico encontrada en los valores de metadatos
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Inicializa una nueva instancia de la clase MetadataSearchRedaction, usando el valor para coincidir con los elementos redactados.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar. |
| replacement | `str` | Reemplazo textual. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Redactar cualquier dirección de correo electrónico en los metadatos
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Inicializa una nueva instancia de MetadataSearchRedaction usando el nombre y el valor del elemento para coincidir con los elementos redactados.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar el valor del elemento de metadatos. |
| replacement | `str` | Reemplazo textual. |
| key_regex | `System.Text.RegularExpressions.Regex` | Expresión regular para buscar y reemplazar el nombre del elemento de metadatos. |

### Ejemplo

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Redactar direcciones de correo electrónico en los valores de metadatos
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Ver también
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
