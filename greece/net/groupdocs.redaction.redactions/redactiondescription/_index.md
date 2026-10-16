---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει πληροφορίες μιας μοναδικής ενέργειας αλλαγής που εκτελέστηκε κατά τη διαδικασία διαγραφής."
type: docs
weight: 720
url: /el/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Αντιπροσωπεύει πληροφορίες μιας μοναδικής ενέργειας αλλαγής που εκτελέστηκε κατά τη διαδικασία διαγραφής.

```csharp
public class RedactionDescription
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription με πληροφορίες αντικατάστασης περιοχής εικόνας. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription με πληροφορίες αντικατάστασης. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Λαμβάνει τη λειτουργία διαγραφής: αντικατάσταση, καθαρισμό ή διαγραφή. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Λαμβάνει ή ορίζει προαιρετικές λεπτομέρειες για το στοιχείο που διαγράφεται. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Λαμβάνει τις πληροφορίες αντικατάστασης για διαγραφές περιοχής εικόνας, επιστρέφει null για διαγραφές κειμένου. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Λαμβάνει το ταιριασμένο κείμενο, εάν έχει δοθεί κάποια έκφραση. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Λαμβάνει τον τύπο των δεδομένων του εγγράφου - κείμενο, μεταδεδομένα ή σημειώσεις. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Λαμβάνει τις πληροφορίες αντικατάστασης, μπορεί να είναι null. |

### Παρατηρήσεις

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
