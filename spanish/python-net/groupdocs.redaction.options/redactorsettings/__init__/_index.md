---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase RedactorSettings."
type: docs
url: /es/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia de la clase RedactorSettings.

```python
def __init__(self):
    ...
```

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#logger}

Inicializa una nueva instancia de RedactorSettings con una instancia de ILogger dada.

```python
def __init__(self, logger):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| logger | `ILogger` | Una instancia de una clase que implementa la interfaz `ILogger`. |

## __init__ {#callback}

Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IRedactionCallback dada.

```python
def __init__(self, callback):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| callback | `IRedactionCallback` | Una instancia de una clase que implementa la interfaz IRedactionCallback. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#ocr_connector}

Inicializa una nueva instancia de RedactorSettings con el IOcrConnector especificado.

```python
def __init__(self, ocr_connector):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Una implementación válida de la interfaz IOcrConnector. |

## __init__ {#logger-callback}

Inicializa una nueva instancia de RedactorSettings con el logger y la devolución de llamada especificados.

```python
def __init__(self, logger, callback):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| logger | `ILogger` | Una instancia de una clase que implementa la interfaz ILogger. |
| callback | `IRedactionCallback` | Una instancia de una clase que implementa la interfaz IRedactionCallback. |

### Ejemplo

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger, IRedactionCallback y IOcrConnector.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| logger | `ILogger` | Una instancia de una clase que implementa la interfaz `ILogger`. |
| callback | `IRedactionCallback` | Una instancia de una clase que implementa la interfaz `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Una instancia de la implementación de la interfaz `IOcrConnector`. Puede ser `None`. |

### Ejemplo

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Ver también
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
