---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe RedactorSettings."
type: docs
url: /fr/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance de la classe RedactorSettings.

```python
def __init__(self):
    ...
```

### Exemple

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

Initialise une nouvelle instance de RedactorSettings avec une instance ILogger donnée.

```python
def __init__(self, logger):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | Une instance d'une classe implémentant l'interface `ILogger`. |

## __init__ {#callback}

Initialise une nouvelle instance de la classe RedactorSettings avec une instance IRedactionCallback donnée.

```python
def __init__(self, callback):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| callback | `IRedactionCallback` | Une instance d'une classe implémentant l'interface IRedactionCallback. |

### Exemple

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

Initialise une nouvelle instance de RedactorSettings avec le IOcrConnector spécifié.

```python
def __init__(self, ocr_connector):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Une implémentation valide de l'interface IOcrConnector. |

## __init__ {#logger-callback}

Initialise une nouvelle instance de RedactorSettings avec le logger et le rappel spécifiés.

```python
def __init__(self, logger, callback):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | Une instance d'une classe implémentant l'interface ILogger. |
| callback | `IRedactionCallback` | Une instance d'une classe implémentant l'interface IRedactionCallback. |

### Exemple

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger, IRedactionCallback et IOcrConnector fournies.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | Une instance d'une classe implémentant l'interface `ILogger`. |
| callback | `IRedactionCallback` | Une instance d'une classe implémentant l'interface `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Une instance de l'implémentation de l'interface `IOcrConnector`. Peut être `None`. |

### Exemple

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Voir aussi
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
