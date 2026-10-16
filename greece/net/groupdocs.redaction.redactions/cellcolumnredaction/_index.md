---
title: "CellColumnRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή κειμένου που αντικαθιστά κείμενο σε έγγραφα λογιστικού φύλλου, CSV, Excel κ.λπ."
type: docs
weight: 540
url: /el/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Αντιπροσωπεύει μια κειμενική απόκρυψη που αντικαθιστά κείμενο σε έγγραφα λογιστικού φύλλου (CSV, Excel, κ.λπ.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης CellColumnRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το [`ReplacementOptions`](../replacementoptions) αντικείμενο, που καθορίζει τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Αποκτά το φίλτρο στήλης και φύλλου εργασίας. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει την υλοποίηση του [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), που απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει την αφαίρεση email χρηστών από τη δεύτερη στήλη στο φύλλο εργασίας "Customers" ενός εγγράφου λογιστικού φύλλου.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // zero-based 2nd column
       WorkSheetName = "Customers"
   };
   var expression = new Regex("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
   RedactorChangeLog changeLog = redactor.Apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
   if (result.Status != RedactionStatus.Failed)
   {
      doc.Save(new SaveOptions() { AddSuffix = true });
   };
}
```

### Δείτε επίσης

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
