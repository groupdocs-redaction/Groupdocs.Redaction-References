---
title: accept_redaction method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Triggered right before applying any redaction to the document, allowing logging or forbidding it."
type: docs
url: /python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Triggered right before applying any redaction to the document, allowing logging or forbidding it.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| description | `RedactionDescription` | Contains information about the particular match type, criteria, text and position. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, RedactorSettings
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

class RedactionLogger:
    def accept_redaction(self, description):
        print(f"{description.redaction_type.name} redaction, original text: {description.original_text}")
        return True

settings = RedactorSettings(RedactionLogger())
with Redactor("sample.docx", LoadOptions(), settings) as redactor:
    redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions("[personal]")))
    redactor.save()
```

### Aliases

These names call `accept_redaction` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `accept_redaction_redaction_description` | `accept_redaction_redaction_description(description)` |

### See Also
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
