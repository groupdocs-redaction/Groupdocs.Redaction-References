---
title: "LoadOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου."
type: docs
weight: 380
url: /el/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου.

```csharp
public class LoadOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions με το καθορισμένο σημαία προ-απόδοση. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions με τον καθορισμένο τύπο αρχείου. |
| [LoadOptions](loadoptions#constructor_3)(string) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions με το καθορισμένο συνθηματικό. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions με το καθορισμένο συνθηματικό. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Λαμβάνει ή ορίζει τον τύπο του αρχείου που θα ανοίξει. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Λαμβάνει ή ορίζει ένα συνθηματικό για έγγραφα με προστασία κωδικού. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το αρχείο θα προ-απόδοση. |

### Παρατηρήσεις

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο με προστασία κωδικού.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // εργασία με έγγραφο
}
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
