---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή κειμένου που αντικαθιστά ακριβή φράση στο κείμενο των εγγράφων χωρίς διάκριση πεζών-κεφαλαίων εξ ορισμού."
type: docs
weight: 600
url: /el/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Αντιπροσωπεύει μια διαγραφή κειμένου που αντικαθιστά ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών-κεφαλαίων. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το [`ReplacementOptions`](../replacementoptions) αντικείμενο, που καθορίζει τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η αναζήτηση είναι με διάκριση πεζών-κεφαλαίων ή όχι. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς τα αριστερά ή όχι, ψευδές εξ ορισμού. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει την υλοποίηση του [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), που απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Λαμβάνει τη συμβολοσειρά για αναζήτηση και αντικατάσταση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει την εκτέλεση αναζήτησης και αντικατάστασης φράσης με διάκριση πεζών-κεφαλαίων.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Από προεπιλογή, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

Το παρακάτω παράδειγμα δείχνει την αντικατάσταση φράσης (χωρίς διάκριση πεζών-κεφαλαίων) με ένα στερεό κόκκινο ορθογώνιο.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Από προεπιλογή, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Δείτε επίσης

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
