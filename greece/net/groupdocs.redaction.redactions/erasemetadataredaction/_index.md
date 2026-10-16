---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή μεταδεδομένων που διαγράφει όλα τα μεταδεδομένα ή τα μεταδεδομένα που ταιριάζουν με συγκεκριμένα MetadataFilters από το έγγραφο."
type: docs
weight: 590
url: /el/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Αντιπροσωπεύει μια διαγραφή μεταδεδομένων που διαγράφει όλα τα μεταδεδομένα ή τα μεταδεδομένα που ταιριάζουν με συγκεκριμένα MetadataFilters από το έγγραφο.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης EraseMetadataRedaction, διαγράφοντας όλα τα μεταδεδομένα. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Αρχικοποιεί μια νέα παρουσία της κλάσης EraseMetadataRedaction, διαγράφοντας μεταδεδομένα, ταιριάζοντας με συγκεκριμένο συνδυασμό του [`MetadataFilters`](../metadatafilters). |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Λαμβάνει ή ορίζει το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Συγγραφέας ή Εταιρεία. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να διαγράψετε (ορίζετε σε κενές τιμές) όλα ή συγκεκριμένα μεταδεδομένα.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Διαγραφή Συγγραφέα, Διευθυντή και Εταιρείας
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Διαγραφή όλων των μεταδεδομένων
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Δείτε επίσης

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
