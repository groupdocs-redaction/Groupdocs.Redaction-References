---
title: "metodo accept_redaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Viene attivato subito prima di applicare qualsiasi redazione al documento, consentendo la registrazione o il suo divieto."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Viene attivato subito prima di applicare qualsiasi redazione al documento, consentendo la registrazione o il suo divieto.

```python
def accept_redaction(self, description):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| description | `RedactionDescription` | Contiene informazioni sul tipo di corrispondenza, i criteri, il testo e la posizione. |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
