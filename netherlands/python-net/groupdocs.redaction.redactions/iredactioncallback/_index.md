---
title: "IRedactionCallback klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Definieert de methoden die nodig zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Definieert de methoden die nodig zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen.

Meer informatie:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Het type IRedactionCallback biedt de volgende leden:

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Activeert vlak voor het toepassen van een redactie op het document, waardoor loggen of verbieden mogelijk is. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
