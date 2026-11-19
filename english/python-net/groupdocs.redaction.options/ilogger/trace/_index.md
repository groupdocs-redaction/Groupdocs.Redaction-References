---
title: trace method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Logs an event that occurred during the redaction process."
type: docs
url: /python-net/groupdocs.redaction.options/ilogger/trace/
is_root: false
weight: 1020
---


## trace {#message}

Logs an event that occurred during the redaction process.

```python
def trace(self, message):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| message | `str` | The event message. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, RedactorSettings
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

class CustomLogger:
    def __init__(self):
        self.traces = []

    def trace(self, message):
        self.traces.append(message)

logger = CustomLogger()
with Redactor("sample.docx", LoadOptions(), RedactorSettings(logger=logger)) as redactor:
    redactor.apply(DeleteAnnotationRedaction())
    # add other redactions as needed
    for msg in logger.traces:
        print("trace:", msg)
```

### Aliases

These names call `trace` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `trace_file` | `trace_file(message)` |
| `trace_string` | `trace_string(message)` |

### See Also
* class [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/)
