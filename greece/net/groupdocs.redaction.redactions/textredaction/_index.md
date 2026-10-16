---
title: "TextRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διαγραφές κειμένου εγγράφου."
type: docs
weight: 800
url: /el/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διαγραφές κειμένου εγγράφου.

```csharp
public abstract class TextRedaction : Redaction
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το [`ReplacementOptions`](../replacementoptions) αντικείμενο, που καθορίζει τον τύπο αντικατάστασης κειμένου. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει την υλοποίηση του [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), που απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
