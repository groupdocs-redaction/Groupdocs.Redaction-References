---
title: "accept_redaction methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Activeert vlak voor het toepassen van een redactie op het document, waardoor loggen of verbieden mogelijk is."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Activeert vlak voor het toepassen van een redactie op het document, waardoor loggen of verbieden mogelijk is.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| description | `RedactionDescription` | Bevat informatie over een specifiek type overeenkomst, criteria, tekst en positie. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Voorbeeld

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

### Zie ook
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
