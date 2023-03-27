---
title: ExactPhraseRedaction
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια επεξεργασία κειμένου που αντικαθιστά την ακριβή φράση στο κείμενο του εγγράφου χωρίς διάκριση πεζώνκεφαλαίων από προεπιλογή.
type: docs
weight: 490
url: /el/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Αντιπροσωπεύει μια επεξεργασία κειμένου που αντικαθιστά την ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction σε λειτουργία μη ευαίσθητης περίπτωσης. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το[`ReplacementOptions`](../replacementoptions) παράδειγμα, προσδιορίζοντας τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά, που περιγράφει τη διόρθωση και τις παραμέτρους της. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η αναζήτηση γίνεται διάκριση πεζών-κεφαλαίων ή όχι. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει το[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) υλοποίηση, που απαιτείται για την εξαγωγή κειμένου από περιεχόμενο γραφικών. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Λαμβάνει τη συμβολοσειρά για αναζήτηση και αντικατάσταση. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει τη διόρθωση σε μια δεδομένη παρουσία μορφής. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Περισσότερες λεπτομέρειες σχετικά με τις διορθώσεις κειμένου εγγράφων: [Διασκευές κειμένων](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει την εκτέλεση αναζήτησης και αντικατάστασης φράσεων με διάκριση πεζών-κεφαλαίων. Το ακόλουθο παράδειγμα δείχνει την αντικατάσταση της φράσης (χωρίς διάκριση πεζών-κεφαλαίων) με συμπαγές κόκκινο ορθογώνιο.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Από προεπιλογή, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Από προεπιλογή, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
  doc.Save();
}
```

### Δείτε επίσης

* class [TextRedaction](../textredaction)
* χώρος ονομάτων [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->