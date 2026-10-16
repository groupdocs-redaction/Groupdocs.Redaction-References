---
title: "FromExtension"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιστοιχίζει την επέκταση αρχείου στον τύπο αρχείου."
type: docs
weight: 500
url: /el/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Αντιστοιχίζει την επέκταση αρχείου στον τύπο αρχείου.

```csharp
public static FileType FromExtension(string extension)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| επέκταση | String | Επέκταση αρχείου (συμπεριλαμβανομένου του σημείου "."). |

### Τιμή Επιστροφής

Όταν ο τύπος αρχείου υποστηρίζεται, το επιστρέφει· διαφορετικά επιστρέφει τον προεπιλεγμένο [`Unknown`](../unknown) τύπο αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Εκτοπίζεται όταν *extension* είναι null ή κενή συμβολοσειρά. |

### Δείτε επίσης

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
