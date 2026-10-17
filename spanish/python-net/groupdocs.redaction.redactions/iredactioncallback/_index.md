---
title: "Clase IRedactionCallback"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Define los métodos necesarios para recibir información sobre cada cambio de redacción y, opcionalmente, evitarlo."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Define los métodos necesarios para recibir información sobre cada cambio de redacción y, opcionalmente, evitarlo.

Más información:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

El tipo IRedactionCallback expone los siguientes miembros:

### Métodos
| Método | Descripción |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Se dispara justo antes de aplicar cualquier redacción al documento, permitiendo registrar o prohibirla. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### Ejemplo

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

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
