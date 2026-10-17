---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der Klasse RedactorSettings."
type: docs
url: /de/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue Instanz der Klasse RedactorSettings.

```python
def __init__(self):
    ...
```

### Beispiel

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

Initialisiert eine neue RedactorSettings-Instanz mit einer angegebenen ILogger-Instanz.

```python
def __init__(self, logger):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| logger | `ILogger` | Eine Instanz einer Klasse, die das `ILogger`-Interface implementiert. |

## __init__ {#callback}

Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IRedactionCallback-Instanz.

```python
def __init__(self, callback):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| callback | `IRedactionCallback` | Eine Instanz einer Klasse, die das IRedactionCallback-Interface implementiert. |

### Beispiel

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

Initialisiert eine neue RedactorSettings-Instanz mit dem angegebenen IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Eine gültige Implementierung des IOcrConnector-Interfaces. |

## __init__ {#logger-callback}

Initialisiert eine neue RedactorSettings-Instanz mit dem angegebenen Logger und Callback.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| logger | `ILogger` | Eine Instanz einer Klasse, die das ILogger-Interface implementiert. |
| callback | `IRedactionCallback` | Eine Instanz einer Klasse, die das IRedactionCallback-Interface implementiert. |

### Beispiel

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Initialisiert eine neue Instanz der Klasse RedactorSettings mit den angegebenen ILogger-, IRedactionCallback- und IOcrConnector-Instanzen.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| logger | `ILogger` | Eine Instanz einer Klasse, die das `ILogger`-Interface implementiert. |
| callback | `IRedactionCallback` | Eine Instanz einer Klasse, die das `IRedactionCallback`-Interface implementiert. |
| ocr_connector | `IOcrConnector` | Eine Instanz einer `IOcrConnector`-Interface-Implementierung. Kann `None` sein. |

### Beispiel

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Siehe auch
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
