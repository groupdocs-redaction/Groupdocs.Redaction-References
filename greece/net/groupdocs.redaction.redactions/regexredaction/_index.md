---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή κειμένου που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση."
type: docs
weight: 750
url: /el/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Αντιπροσωπεύει μια διαγραφή κειμένου που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση.

```csharp
public class RegexRedaction : TextRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegexRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το [`ReplacementOptions`](../replacementoptions) αντικείμενο, που καθορίζει τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει την υλοποίηση του [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), που απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει την αντικατάσταση κειμένου χρησιμοποιώντας την κανονική έκφραση.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // αντικατάσταση με κείμενο
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // αντικατάσταση με μπλε στερεό ορθογώνιο
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Δείτε επίσης

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
