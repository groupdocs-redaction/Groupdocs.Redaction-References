---
title: "Classe IRedactionCallback"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Definisce i metodi necessari per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Definisce i metodi necessari per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla.

Per saperne di più:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Il tipo IRedactionCallback espone i seguenti membri:

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Viene attivato subito prima di applicare qualsiasi redazione al documento, consentendo la registrazione o il suo divieto. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### Esempio

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

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
