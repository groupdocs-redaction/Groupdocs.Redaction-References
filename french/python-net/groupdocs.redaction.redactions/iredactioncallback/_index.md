---
title: "Classe IRedactionCallback"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et, éventuellement, l'empêcher."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et, éventuellement, l'empêcher.

En savoir plus :
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Le type IRedactionCallback expose les membres suivants :

### Méthodes
| Méthode | Description |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Se déclenche juste avant d'appliquer une quelconque censure au document, permettant la journalisation ou son interdiction. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
