---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of the RedactorSettings class."
type: docs
url: /python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the RedactorSettings class.

```python
def __init__(self):
    ...
```

### Example

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

Initializes a new RedactorSettings instance with a given ILogger instance.

```python
def __init__(self, logger):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing the `ILogger` interface. |

## __init__ {#callback}

Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance.

```python
def __init__(self, callback):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| callback | `IRedactionCallback` | An instance of a class implementing IRedactionCallback interface. |

### Example

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

Initializes a new RedactorSettings instance with the specified IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | A valid implementation of IOcrConnector interface. |

## __init__ {#logger-callback}

Initializes a new RedactorSettings instance with the specified logger and callback.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing the ILogger interface. |
| callback | `IRedactionCallback` | An instance of a class implementing the IRedactionCallback interface. |

### Example

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing `ILogger` interface. |
| callback | `IRedactionCallback` | An instance of a class implementing `IRedactionCallback` interface. |
| ocr_connector | `IOcrConnector` | An instance of `IOcrConnector` interface implementation. Can be `None`. |

### Example

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### See Also
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
