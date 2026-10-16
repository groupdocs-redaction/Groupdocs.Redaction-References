---
title: "MetadataSearchRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή μεταδεδομένων που αναζητά και διαγράφει μεταδεδομένα χρησιμοποιώντας κανονικές εκφράσεις που ταιριάζουν με κλειδιά και/ή τιμές."
type: docs
weight: 660
url: /el/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Αντιπροσωπεύει μια διαγραφή μεταδεδομένων που αναζητά και διαγράφει μεταδεδομένα χρησιμοποιώντας κανονικές εκφράσεις, ταιριάζοντας κλειδιά και/ή τιμές.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας τιμή για την αντιστοίχιση των αντικειμένων που διαγράφονται. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας τιμή για την αντιστοίχιση των αντικειμένων που διαγράφονται. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας το όνομα του αντικειμένου και την τιμή για την αντιστοίχιση των αντικειμένων που διαγράφονται. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας το όνομα του αντικειμένου και την τιμή για την αντιστοίχιση των αντικειμένων που διαγράφονται. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Λαμβάνει ή ορίζει το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Συγγραφέας ή Εταιρεία. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Λαμβάνει την κανονική έκφραση για την αντιστοίχιση του ονόματος (κλειδιού) ενός αντικειμένου μεταδεδομένων. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Λαμβάνει την τιμή αντικατάστασης κειμένου. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Λαμβάνει την κανονική έκφραση για την αντιστοίχιση του κειμένου τιμής ενός αντικειμένου μεταδεδομένων. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αναζητήσετε και να διαγράψετε συγκεκριμένο κείμενο σε συγκεκριμένα μεταδεδομένα.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Εάν δεν οριστεί, εφαρμόζεται σε όλα τα στοιχεία μεταδεδομένων
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Δείτε επίσης

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
