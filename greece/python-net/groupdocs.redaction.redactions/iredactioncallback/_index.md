---
title: "κλάση IRedactionCallback"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Ορίζει τις μεθόδους που απαιτούνται για τη λήψη πληροφοριών σχετικά με κάθε αλλαγή επεξεργασίας και προαιρετικά την αποτροπή της."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Ορίζει τις μεθόδους που απαιτούνται για τη λήψη πληροφοριών σχετικά με κάθε αλλαγή επεξεργασίας και προαιρετικά την αποτροπή της.

Μάθετε περισσότερα:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Ο τύπος IRedactionCallback εκθέτει τα ακόλουθα μέλη:

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Ενεργοποιείται ακριβώς πριν την εφαρμογή οποιασδήποτε διαγραφής στο έγγραφο, επιτρέποντας την καταγραφή ή την απαγόρευσή της. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### Παράδειγμα

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

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
