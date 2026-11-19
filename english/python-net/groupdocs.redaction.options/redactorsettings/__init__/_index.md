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

## __init__ {#logger}

Initializes a new RedactorSettings instance with the specified logger.

```python
def __init__(self, logger):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing the ILogger interface. |

### Example

```python
from groupdocs.redaction.options import RedactorSettings

class Log:
    def __init__(self):
        self.errors, self.traces = [], []

    def error(self, message):
        self.errors.append(message)

    def warning(self, message):
        pass

    def trace(self, message):
        self.traces.append(message)

log = Log()
settings = RedactorSettings(logger=log)
```

## __init__ {#callback}

Initializes a new RedactorSettings instance with a given IRedactionCallback implementation.

```python
def __init__(self, callback):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| callback | `IRedactionCallback` | An instance of a class implementing the `IRedactionCallback` interface. |

### Example

```python
from groupdocs.redaction.options import RedactorSettings

def accept_first_only(description):
    # Accept only the first redaction change
    return True

# Create settings with a callback function
settings = RedactorSettings(callback=accept_first_only)
```

## __init__ {#ocr_connector}

Initializes a new RedactorSettings instance with the specified IOcrConnector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | A valid implementation of the IOcrConnector interface. |

## __init__ {#logger-callback}

Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing the ILogger interface. |
| callback | `IRedactionCallback` | An instance of a class implementing the IRedactionCallback interface. |

## __init__ {#logger-callback-ocr_connector}

Initializes a new [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/) instance with optional logger, callback, and OCR connector.

The `logger` argument should be an object implementing the [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) interface.  
The `callback` argument should be an object implementing the [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface.  
The `ocr_connector` argument should implement [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/); it may be `None` when OCR integration is not required.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class implementing the `ILogger` interface. |
| callback | `IRedactionCallback` | An instance of a class implementing the `IRedactionCallback` interface. |
| ocr_connector | `IOcrConnector` | An instance of an `IOcrConnector` implementation, or `None`. |

### Example

```python
from groupdocs.redaction.options import RedactorSettings

class Log:
    def error(self, message): pass
    def warning(self, message): pass
    def trace(self, message): pass

def accept_first_only(description):
    # Accept only the first redaction change
    return len(description.original_text) > 0

# Create settings with a logger, a callback function, and no OCR connector
settings = RedactorSettings(logger=Log(), callback=accept_first_only, ocr_connector=None)
```

### See Also
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
