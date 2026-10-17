---
title: "μέθοδος accept_redaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Ενεργοποιείται ακριβώς πριν την εφαρμογή οποιασδήποτε διαγραφής στο έγγραφο, επιτρέποντας την καταγραφή ή την απαγόρευσή της."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Ενεργοποιείται ακριβώς πριν την εφαρμογή οποιασδήποτε διαγραφής στο έγγραφο, επιτρέποντας την καταγραφή ή την απαγόρευσή της.

```python
def accept_redaction(self, description):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| description | `RedactionDescription` | Περιέχει πληροφορίες σχετικά με συγκεκριμένο τύπο αντιστοίχισης, κριτήρια, κείμενο και θέση. |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
