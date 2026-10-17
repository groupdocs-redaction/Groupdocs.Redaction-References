---
title: "accept_redaction Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Wird unmittelbar vor dem Anwenden einer Redaktion auf das Dokument ausgelöst und ermöglicht das Protokollieren oder das Verhindern."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Wird unmittelbar vor dem Anwenden einer Redaktion auf das Dokument ausgelöst und ermöglicht das Protokollieren oder das Verhindern.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| description | `RedactionDescription` | Enthält Informationen über den jeweiligen Übereinstimmungstyp, das Kriterium, den Text und die Position. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Beispiel

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

### Siehe auch
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
