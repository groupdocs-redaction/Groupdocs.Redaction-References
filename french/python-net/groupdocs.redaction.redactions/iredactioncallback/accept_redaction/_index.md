---
title: "méthode accept_redaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Se déclenche juste avant d'appliquer une quelconque censure au document, permettant la journalisation ou son interdiction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Se déclenche juste avant d'appliquer une quelconque censure au document, permettant la journalisation ou son interdiction.

```python
def accept_redaction(self, description):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| description | `RedactionDescription` | Contient des informations sur le type de correspondance particulier, les critères, le texte et la position. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Exemple

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

### Voir aussi
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
