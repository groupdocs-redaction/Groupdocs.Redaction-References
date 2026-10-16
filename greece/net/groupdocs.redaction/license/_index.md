---
title: "License"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει μεθόδους για την εφαρμογή άδειας."
type: docs
weight: 270
url: /el/net/groupdocs.redaction/license/
---
## License class

Παρέχει μεθόδους για την εφαρμογή άδειας.

```csharp
public class License
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [License](license)() | Αρχικοποιεί μια παρουσία της κλάσης License. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Ορίζει την άδεια GroupDocs.Redaction από μια ροή. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Ορίζει την άδεια GroupDocs.Redaction από διαδρομή αρχείου. |

### Παρατηρήσεις

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ορίσετε την άδεια για το GroupDocs.Redaction.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// ως εναλλακτική, μπορείτε να χρησιμοποιήσετε μια ροή:
license.SetLicense(licensePath);
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
