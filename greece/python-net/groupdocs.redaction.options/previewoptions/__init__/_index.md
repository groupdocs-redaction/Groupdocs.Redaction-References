---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο PreviewOptions."
type: docs
url: /el/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Αρχικοποιεί ένα νέο αντικείμενο PreviewOptions. Η ροή εξόδου θα κλείσει μετά τη χρήση.

```python
def __init__(self, create_page_stream):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας. |

## __init__ {#create_page_stream-release_page_stream}

Αρχικοποιεί ένα νέο αντικείμενο PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας. |
| release_page_stream | `ReleasePageStream` | Ειδοποιεί ότι η δημιουργία προεπισκόπησης σελίδας ολοκληρώθηκε και λαμβάνει το output stream. |

### Δείτε επίσης
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
