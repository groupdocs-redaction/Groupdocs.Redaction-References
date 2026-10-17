---
title: "accept_redaction método"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Se dispara justo antes de aplicar cualquier redacción al documento, permitiendo registrar o prohibirla."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Se dispara justo antes de aplicar cualquier redacción al documento, permitiendo registrar o prohibirla.

```python
def accept_redaction(self, description):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| description | `RedactionDescription` | Contiene información sobre el tipo de coincidencia particular, criterios, texto y posición. |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
