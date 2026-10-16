---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια λίστα των πιο κοινών τύπων μεταδεδομένων εγγράφου."
type: docs
weight: 640
url: /el/net/groupdocs.redaction.redactions/metadatafilters/
---
## MetadataFilters enumeration

Αντιπροσωπεύει μια λίστα των πιο κοινών τύπων μεταδεδομένων εγγράφου.

```csharp
[Flags]
public enum MetadataFilters
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Κενή ρύθμιση φίλτρου, δεν ταιριάζει με κανένα στοιχείο μεταδεδομένων. |
| Author | `1` | Συγγραφέας του εγγράφου. |
| Category | `2` | Κατηγορία του εγγράφου. |
| Comments | `4` | Σχόλιο για το έγγραφο. |
| Company | `8` | Εταιρεία του Συγγραφέα. |
| ContentStatus | `10` | Κατάσταση περιεχομένου. |
| CreatedTime | `20` | Ώρα δημιουργίας. |
| HyperlinkBase | `40` | Βάση υπερσυνδέσμου. |
| LastPrinted | `80` | Τελευταία ημερομηνία και ώρα εκτύπωσης. |
| LastSavedBy | `100` | Τελευταία αποθήκευση από τον χρήστη. |
| LastSavedTime | `400` | Τελευταία ημερομηνία και ώρα αποθήκευσης. |
| NameOfApplication | `800` | Όνομα της εφαρμογής όπου δημιουργήθηκε το έγγραφο. |
| Manager | `1000` | Όνομα του διευθυντή του συγγραφέα. |
| RevisionNumber | `2000` | Αριθμός αναθεώρησης. |
| Subject | `4000` | Θέμα του εγγράφου. |
| Template | `8000` | Όνομα προτύπου εγγράφου. |
| Title | `10000` | Τίτλος εγγράφου. |
| TotalEditingTime | `20000` | Συνολικός χρόνος επεξεργασίας. |
| Version | `40000` | Έκδοση εγγράφου. |
| Description | `80000` | Περιγραφή εγγράφου. |
| Keywords | `100000` | Λέξεις-κλειδιά εγγράφου. |
| ContentType | `200000` | Τύπος περιεχομένου. |
| All | `7FFFFFFF` | Όλοι οι τύποι των στοιχείων μεταδεδομένων. |

### Παρατηρήσεις

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
