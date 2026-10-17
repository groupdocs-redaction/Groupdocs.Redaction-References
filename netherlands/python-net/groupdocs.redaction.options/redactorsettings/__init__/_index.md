---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van de RedactorSettings-klasse."
type: docs
url: /nl/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuw exemplaar van de RedactorSettings-klasse.

```python
def __init__(self):
    ...
```

### Voorbeeld

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

Initialiseert een nieuw RedactorSettings-exemplaar met een gegeven ILogger-instantie.

```python
def __init__(self, logger):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| logger | `ILogger` | Een instantie van een klasse die de `ILogger`-interface implementeert. |

## __init__ {#callback}

Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een gegeven IRedactionCallback-instantie.

```python
def __init__(self, callback):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| callback | `IRedactionCallback` | Een instantie van een klasse die de IRedactionCallback-interface implementeert. |

### Voorbeeld

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

Initialiseert een nieuw RedactorSettings-exemplaar met de opgegeven IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Een geldige implementatie van de IOcrConnector-interface. |

## __init__ {#logger-callback}

Initialiseert een nieuw RedactorSettings-exemplaar met de opgegeven logger en callback.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| logger | `ILogger` | Een instantie van een klasse die de ILogger-interface implementeert. |
| callback | `IRedactionCallback` | Een instantie van een klasse die de IRedactionCallback‑interface implementeert. |

### Voorbeeld

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger-, IRedactionCallback- en IOcrConnector-instanties.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| logger | `ILogger` | Een instantie van een klasse die de `ILogger`‑interface implementeert. |
| callback | `IRedactionCallback` | Een instantie van een klasse die de `IRedactionCallback`‑interface implementeert. |
| ocr_connector | `IOcrConnector` | Een instantie van een `IOcrConnector`‑interface‑implementatie. Kan `None` zijn. |

### Voorbeeld

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Zie ook
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
