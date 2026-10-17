---
title: "μέθοδος set_license"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Εφαρμόστε μια άδεια στη τρέχουσα διεργασία."
type: docs
url: /el/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

Εφαρμόστε μια άδεια στη τρέχουσα διεργασία.

```python
def set_license(self, license_source):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| license_source |  | Είτε μια διαδρομή συμβολοσειράς προς ένα αρχείο ``.lic`` είτε ένα αναγνώσιμο αντικείμενο τύπου αρχείου που παρέχει τα bytes της άδειας. Τα εισερχόμενα τύπου αρχείου γράφονται σε ένα προσωρινό αρχείο πριν περάσουν στη γέφυρα. |

| Αναφέρει | Περιγραφή |
| :- | :- |
| `TypeError` | Εάν το ``license_source`` δεν είναι ούτε διαδρομή συμβολοσειράς ούτε αναγνώσιμο αντικείμενο τύπου αρχείου. |

### Δείτε επίσης
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
