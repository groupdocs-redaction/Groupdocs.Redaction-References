---
title: RegexRedaction
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια επεξεργασία κειμένου που αναζητά και αντικαθιστά κείμενο στο έγγραφο αντιστοιχίζοντας την παρεχόμενη κανονική έκφραση.
type: docs
weight: 590
url: /el/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Αντιπροσωπεύει μια επεξεργασία κειμένου που αναζητά και αντικαθιστά κείμενο στο έγγραφο αντιστοιχίζοντας την παρεχόμενη κανονική έκφραση.

```csharp
public class RegexRedaction : TextRedaction
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το[`ReplacementOptions`](../replacementoptions) παράδειγμα, προσδιορίζοντας τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά, που περιγράφει τη διόρθωση και τις παραμέτρους της. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει το[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) υλοποίηση, που απαιτείται για την εξαγωγή κειμένου από περιεχόμενο γραφικών. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Παίρνει την τυπική έκφραση για να ταιριάζει. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει τη διόρθωση σε μια δεδομένη παρουσία μορφής. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Περισσότερες λεπτομέρειες σχετικά με τις διορθώσεις κειμένου εγγράφων: [Διασκευές κειμένων](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει την αντικατάσταση κειμένου χρησιμοποιώντας την κανονική έκφραση.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // αντικατάσταση με κείμενο
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // αντικαταστήστε με μπλε συμπαγές ορθογώνιο
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(System.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Δείτε επίσης

* class [TextRedaction](../textredaction)
* χώρος ονομάτων [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
