---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe RedactorSettings."
type: docs
url: /it/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza della classe RedactorSettings.

```python
def __init__(self):
    ...
```

### Esempio

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

Inizializza una nuova istanza di RedactorSettings con una data istanza di ILogger.

```python
def __init__(self, logger):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| logger | `ILogger` | Un'istanza di una classe che implementa l'interfaccia `ILogger`. |

## __init__ {#callback}

Inizializza una nuova istanza della classe RedactorSettings con una data istanza di IRedactionCallback.

```python
def __init__(self, callback):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| callback | `IRedactionCallback` | Un'istanza di una classe che implementa l'interfaccia IRedactionCallback. |

### Esempio

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

Inizializza una nuova istanza di RedactorSettings con l'IOcrConnector specificato.

```python
def __init__(self, ocr_connector):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Una valida implementazione dell'interfaccia IOcrConnector. |

## __init__ {#logger-callback}

Inizializza una nuova istanza di RedactorSettings con il logger e il callback specificati.

```python
def __init__(self, logger, callback):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| logger | `ILogger` | Un'istanza di una classe che implementa l'interfaccia ILogger. |
| callback | `IRedactionCallback` | Un'istanza di una classe che implementa l'interfaccia IRedactionCallback. |

### Esempio

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Inizializza una nuova istanza della classe RedactorSettings con le istanze di ILogger, IRedactionCallback e IOcrConnector fornite.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| logger | `ILogger` | Un'istanza di una classe che implementa l'interfaccia `ILogger`. |
| callback | `IRedactionCallback` | Un'istanza di una classe che implementa l'interfaccia `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Un'istanza dell'implementazione dell'interfaccia `IOcrConnector`. Può essere `None`. |

### Esempio

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Vedi anche
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
