---
title: "redact μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Εφαρμόζει προσαρμοσμένη διαγραφή σε συγκεκριμένο περιεχόμενο εγγράφου."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Εφαρμόζει προσαρμοσμένη διαγραφή σε συγκεκριμένο περιεχόμενο εγγράφου.

Προς το παρόν, αυτό υποστηρίζεται μόνο για PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Οι χρήστες μπορούν να ορίσουν τη δική τους λογική σήμανσης, όπως η σήμανση με τεχνητή νοημοσύνη, η οποία μπορεί να είναι πιο προχωρημένη από τις απλές μεθόδους βασισμένες σε μοτίβα.

```python
def redact(self, context):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| context | `CustomRedactionContext` | Περιέχει το περιεχόμενο του εγγράφου που θα σημαδευτεί μαζί με τα σχετικά μεταδεδομένα. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Δείτε επίσης
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
