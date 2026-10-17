---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av klassen RedactorSettings."
type: docs
url: /sv/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny instans av klassen RedactorSettings.

```python
def __init__(self):
    ...
```

### Exempel

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

Initierar en ny RedactorSettings-instans med en given ILogger-instans.

```python
def __init__(self, logger):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| logger | `ILogger` | En instans av en klass som implementerar `ILogger`-gränssnittet. |

## __init__ {#callback}

Initierar en ny instans av klassen RedactorSettings med en given IRedactionCallback-instans.

```python
def __init__(self, callback):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| callback | `IRedactionCallback` | En instans av en klass som implementerar IRedactionCallback-gränssnittet. |

### Exempel

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

Initierar en ny RedactorSettings-instans med den angivna IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | En giltig implementation av IOcrConnector-gränssnittet. |

## __init__ {#logger-callback}

Initierar en ny RedactorSettings-instans med den angivna logger och callback.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| logger | `ILogger` | En instans av en klass som implementerar ILogger-gränssnittet. |
| callback | `IRedactionCallback` | En instans av en klass som implementerar IRedactionCallback-gränssnittet. |

### Exempel

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Initierar en ny instans av klassen RedactorSettings med givna ILogger-, IRedactionCallback- och IOcrConnector-instans.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| logger | `ILogger` | En instans av en klass som implementerar `ILogger`-gränssnittet. |
| callback | `IRedactionCallback` | En instans av en klass som implementerar `IRedactionCallback`-gränssnittet. |
| ocr_connector | `IOcrConnector` | En instans av `IOcrConnector`-gränssnittets implementation. Kan vara `None`. |

### Exempel

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Se även
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
