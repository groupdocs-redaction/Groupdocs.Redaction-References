---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια σύνθετη διαγραφή κειμένου που επηρεάζει κείμενα, εικόνες και σημειώσεις σε μια περιοχή της σελίδας."
type: docs
weight: 680
url: /el/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Αντιπροσωπεύει μια σύνθετη κειμενική διαγραφή που επηρεάζει κείμενο, εικόνες και σημειώσεις σε μια περιοχή της σελίδας.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PageAreaRedaction. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PageAreaRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Λαμβάνει το [`ReplacementOptions`](../replacementoptions) αντικείμενο, που καθορίζει τον τύπο αντικατάστασης κειμένου. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Λαμβάνει τις επιλογές [`RegionReplacementOptions`](../regionreplacementoptions) με χρώμα και παραμέτρους περιοχής. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει την υλοποίηση του [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), που απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Δείτε επίσης

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
