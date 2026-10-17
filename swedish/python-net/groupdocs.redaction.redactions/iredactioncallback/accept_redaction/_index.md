---
title: "accept_redaction-metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Utlöses precis innan någon redigering tillämpas på dokumentet, vilket möjliggör loggning eller förbud."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Utlöses precis innan någon redigering tillämpas på dokumentet, vilket möjliggör loggning eller förbud.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| description | `RedactionDescription` | Innehåller information om specifik matchningstyp, kriterier, text och position. |

**Returns:** bool: True to accept the redaction, False to decline it.

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

### Se även
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
