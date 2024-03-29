---
title: RemovePageRedaction
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια διόρθωση που αφαιρεί μια σελίδα διαφάνεια φύλλο εργασίας κ.λπ. από ένα έγγραφο.
type: docs
weight: 610
url: /el/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Αντιπροσωπεύει μια διόρθωση που αφαιρεί μια σελίδα (διαφάνεια, φύλλο εργασίας, κ.λπ.) από ένα έγγραφο.

```csharp
public class RemovePageRedaction : Redaction
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Αρχικοποιεί μια νέα παρουσία της κλάσης RemovePageRedaction. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Λαμβάνει τον αριθμό των σελίδων προς κατάργηση. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Επιστρέφει μια συμβολοσειρά, που περιγράφει τη διόρθωση και τις παραμέτρους της. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Λήψη δείκτη θέσης έναρξης (βάσει 0). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Λαμβάνει θέση αναφοράς αναζήτησης, την αρχή ή το τέλος ενός εγγράφου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει τη διόρθωση σε μια δεδομένη παρουσία μορφής. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Περισσότερες λεπτομέρειες σχετικά με την κατάργηση σελίδων: [Κατάργηση διόρθωσης σελίδας](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να αφαιρέσετε την τελευταία σελίδα του εγγράφου.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* χώρος ονομάτων [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
