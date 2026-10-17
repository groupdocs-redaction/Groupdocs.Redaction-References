---
title: "IRedactionCallback Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Definiert die für das Empfangen von Informationen zu jeder Redaktionsänderung erforderlichen Methoden und verhindert sie optional."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Definiert die für das Empfangen von Informationen zu jeder Redaktionsänderung erforderlichen Methoden und verhindert sie optional.

Mehr erfahren:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Der Typ IRedactionCallback stellt die folgenden Mitglieder bereit:

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Wird unmittelbar vor dem Anwenden einer Redaktion auf das Dokument ausgelöst und ermöglicht das Protokollieren oder das Verhindern. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
