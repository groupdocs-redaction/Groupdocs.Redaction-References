---
title: accept_redaction method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Triggers right before applying any redaction to the document, allowing logging or forbidding it."
type: docs
url: /python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Triggers right before applying any redaction to the document, allowing logging or forbidding it.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| description | `RedactionDescription` | Contains information about particular match type, criteria, text and position. |

**Returns:** bool: True to accept the redaction, False to decline it.

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

### See Also
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
