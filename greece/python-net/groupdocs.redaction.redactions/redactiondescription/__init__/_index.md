---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redaction_type | `RedactionType` | Τύπος των δεδομένων που διαγράφονται. |
| action_type | `RedactionActionType` | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα. |
| original_text | `str` | Ταιριακό κείμενο, σχόλιο ή σώμα σημείωσης. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription με πληροφορίες αντικατάστασης.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redaction_type | `RedactionType` | Τύπος των δεδομένων που διαγράφονται. |
| action_type | `RedactionActionType` | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα. |
| original_text | `str` | Ταιριακό κείμενο, σχόλιο ή σώμα σημείωσης. |
| replacement | `TextReplacement` | Κείμενο αντικατάστασης, ταιριακό κείμενο και η θέση του μέσα στην αρχική συμβολοσειρά. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Αρχικοποιεί ένα νέο RedactionDescription με πληροφορίες αντικατάστασης περιοχής εικόνας.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redaction_type | `RedactionType` | Τύπος των δεδομένων που διαγράφονται. |
| action_type | `RedactionActionType` | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα. |
| image_area_replacement | `RegionReplacementOptions` | Πληροφορίες αντικατάστασης περιοχής εικόνας. |
| image_details | `str` | Κειμενική περιγραφή εικόνας, εξ ορισμού είναι κενή συμβολοσειρά. |

### Δείτε επίσης
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
