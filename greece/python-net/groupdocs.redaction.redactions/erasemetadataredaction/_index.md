---
title: "Κλάση EraseMetadataRedaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια απόκρυψη μεταδεδομένων που διαγράφει όλα τα μεταδεδομένα ή τα μεταδεδομένα που ταιριάζουν με συγκεκριμένα MetadataFilters από το έγγραφο."
type: docs
url: /el/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Αντιπροσωπεύει μια απόκρυψη μεταδεδομένων που διαγράφει όλα τα μεταδεδομένα ή τα μεταδεδομένα που ταιριάζουν με συγκεκριμένα MetadataFilters από το έγγραφο.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Ο τύπος EraseMetadataRedaction εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης EraseMetadataRedaction, διαγράφοντας όλα τα μεταδεδομένα. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Αρχικοποιεί μια νέα παρουσία της EraseMetadataRedaction, διαγράφοντας τα μεταδεδομένα που ταιριάζουν με τα καθορισμένα `MetadataFilters`. |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Εφαρμόζει τη διαγραφή σε μια δεδομένη παρουσία μορφής. (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Η περιγραφή της διαγραφής και των παραμέτρων της. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Το φίλτρο που χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, όπως Συγγραφέας ή Εταιρεία. (κληρονομείται από [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Διαγραφή όλων των μεταδεδομένων
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Διαγραφή μόνο του πεδίου συγγραφέα
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν το `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
