---
title: error method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Logs an error that occurred during redaction process."
type: docs
url: /python-net/groupdocs.redaction.options/ilogger/error/
is_root: false
weight: 1010
---


## error {#message}

Logs an error that occurred during redaction process.

```python
def error(self, message):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| message | `str` | The error message. |

### Example

```python
class CustomLogger:
    def __init__(self):
        self.errors = []

    def error(self, message):
        self.errors.append(message)

logger = CustomLogger()
logger.error("Failed to open the document.")
print(logger.errors)  # ['Failed to open the document.']
```

### Aliases

These names call `error` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `error_file` | `error_file(message)` |
| `error_string` | `error_string(message)` |

### See Also
* class [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/)
