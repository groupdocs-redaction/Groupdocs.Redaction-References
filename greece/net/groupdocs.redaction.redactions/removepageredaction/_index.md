---
title: "RemovePageRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή που αφαιρεί μια σελίδα, διαφάνεια, φύλλο εργασίας κ.λπ. από ένα έγγραφο."
type: docs
weight: 770
url: /el/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Αντιπροσωπεύει μια διαγραφή που αφαιρεί μια σελίδα (διαφάνεια, φύλλο εργασίας κ.λπ.) από ένα έγγραφο.

```csharp
public class RemovePageRedaction : Redaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RemovePageRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Λαμβάνει τον αριθμό των σελίδων προς αφαίρεση. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Λαμβάνει τον δείκτη της αρχικής θέσης (από το 0). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Λαμβάνει τη θέση αναφοράς αναζήτησης, την αρχή ή το τέλος ενός εγγράφου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αφαιρέσετε την τελευταία σελίδα του εγγράφου.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
