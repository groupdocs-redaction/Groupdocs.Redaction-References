---
title: MetadataSearchRedaction
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που πραγματοποιεί αναζήτηση και διόρθωση μεταδεδομένων χρησιμοποιώντας κανονικές εκφράσεις αντιστοιχισμένα κλειδιά και/ή τιμές.
type: docs
weight: 540
url: /el/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που πραγματοποιεί αναζήτηση και διόρθωση μεταδεδομένων χρησιμοποιώντας κανονικές εκφράσεις, αντιστοιχισμένα κλειδιά και/ή τιμές.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των αναγραφόμενων στοιχείων. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας την τιμή για την αντιστοίχιση των αναγραφόμενων στοιχείων. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για αντιστοίχιση των αναγραφόμενων στοιχείων. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης MetadataSearchRedaction, χρησιμοποιώντας το όνομα και την τιμή του στοιχείου για αντιστοίχιση των αναγραφόμενων στοιχείων. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά, που περιγράφει τη διόρθωση και τις παραμέτρους της. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Λαμβάνει ή ορίζει το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Συγγραφέας ή Εταιρεία. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Λαμβάνει την τυπική έκφραση για να ταιριάζει με το όνομα (κλειδί) του στοιχείου μεταδεδομένων. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Λαμβάνει την τιμή αντικατάστασης κειμένου. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Λαμβάνει την τυπική έκφραση για να ταιριάζει με το κείμενο αξίας ενός στοιχείου μεταδεδομένων. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει τη διόρθωση σε μια δεδομένη παρουσία μορφής. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Περισσότερες λεπτομέρειες σχετικά με τις διορθώσεις μεταδεδομένων εγγράφων: [Διασκευές μεταδεδομένων](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει τον τρόπο αναζήτησης και επεξεργασίας συγκεκριμένου κειμένου σε συγκεκριμένα μεταδεδομένα.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Εάν δεν έχει οριστεί, ισχύει για όλα τα στοιχεία μεταδεδομένων
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Δείτε επίσης

* class [MetadataRedaction](../metadataredaction)
* χώρος ονομάτων [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
