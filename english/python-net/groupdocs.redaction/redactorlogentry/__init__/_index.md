---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new RedactorLogEntry for redaction."
type: docs
url: /python-net/groupdocs.redaction/redactorlogentry/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction-result}

Initializes a new RedactorLogEntry for redaction.

All metadata redactions apply to each metadata item separately, and even if a metadata item redaction fails, the rest of the metadata items will be updated. A list of failed, skipped (rejected) metadata items and reasons can be found in the `ErrorMessage` property of [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

```python
def __init__(self, redaction, result):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction | `Redaction` | Reference to the redaction. |
| result | `RedactionResult` | Redaction result reported by the format handler. |

### See Also
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
