---
title: warning method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Logs a warning that occurred during redaction process."
type: docs
url: /python-net/groupdocs.redaction.options/ilogger/warning/
is_root: false
weight: 1030
---


## warning {#message}

Logs a warning that occurred during redaction process.

```python
def warning(self, message):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| message | `str` | The warning message. |

### Example

```python
class CustomLogger:
    def warning(self, message):
        print(f"Warning: {message}")

logger = CustomLogger()
logger.warning("Potential issue detected.")
```

### Aliases

These names call `warning` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `warning_file` | `warning_file(message)` |
| `warning_string` | `warning_string(message)` |

### See Also
* class [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/)
