---
title: "IRedactionCallback-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Definierar metoder som krävs för att ta emot information om varje raderingsändring och eventuellt förhindra den."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Definierar metoder som krävs för att ta emot information om varje raderingsändring och eventuellt förhindra den.

Läs mer:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

IRedactionCallback-typen exponerar följande medlemmar:

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Utlöses precis innan någon redigering tillämpas på dokumentet, vilket möjliggör loggning eller förbud. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### Exempel

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

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
