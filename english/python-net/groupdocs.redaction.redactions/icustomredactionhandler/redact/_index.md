---
title: redact method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Applies custom redaction to specific document content."
type: docs
url: /python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Applies custom redaction to specific document content.

Currently, this is supported only for PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Users can define their own redaction logic, such as AI-based redaction, which may be more advanced than simple pattern-based methods.

```python
def redact(self, context):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| context | `CustomRedactionContext` | Contains the document content to be redacted along with related metadata. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### See Also
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
