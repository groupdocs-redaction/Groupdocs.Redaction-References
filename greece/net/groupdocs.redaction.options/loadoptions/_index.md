---
title: LoadOptions
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου.
type: docs
weight: 310
url: /el/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου.

```csharp
public class LoadOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης LoadOptions. |
| [LoadOptions](loadoptions#constructor_1)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης LoadOptions με καθορισμένο κωδικό πρόσβασης. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για έγγραφα που προστατεύονται με κωδικό πρόσβασης. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Φόρτωση εγγράφων](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Φόρτωση από τοπικό δίσκο](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Φόρτωση από ροή](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Φόρτωση εγγράφου που προστατεύεται με κωδικό πρόσβασης](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // εργασία με έγγραφο
}
```

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
