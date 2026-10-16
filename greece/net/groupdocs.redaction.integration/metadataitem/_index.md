---
title: "MetadataItem"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναπαριστά ένα στοιχείο μεταδεδομένων κοινό για όλες τις υποστηριζόμενες μορφές και χρησιμοποιείται σε επεμβάσεις μεταδεδομένων."
type: docs
weight: 220
url: /el/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Αντιπροσωπεύει ένα στοιχείο μεταδεδομένων, κοινό για όλες τις υποστηριζόμενες μορφές και χρησιμοποιείται σε διαγραφές μεταδεδομένων.

```csharp
public class MetadataItem : ISerializable
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MetadataItem](metadataitem)() | Αρχικοποιεί μια νέα παρουσία. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Επιστρέφει την αναπαράσταση συμβολοσειράς της τιμής του στοιχείου μεταδεδομένων. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Λαμβάνει ή ορίζει μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων πόρου. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Λαμβάνει ένα κλειδί λεξικού για [`MetadataCollection`](../metadatacollection), χρησιμοποιώντας το OriginalName του και άλλα δεδομένα. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Λαμβάνει ή ορίζει μια τιμή του [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters), που έχει ανατεθεί σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στη φιλτράρισμα των στοιχείων. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους δημιουργούς του εγγράφου). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Λαμβάνει ή ορίζει το αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Λαμβάνει ή ορίζει την τιμή του στοιχείου μεταδεδομένων. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Δημιουργεί ένα βαθύ κλώνο της τρέχουσας παρουσίας. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Επιστρέφει πληροφορίες σχετικά με τις σειριοποιήσιμες ιδιότητες. |

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
