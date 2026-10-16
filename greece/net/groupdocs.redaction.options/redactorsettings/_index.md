---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναπαριστά τις ρυθμίσεις απόκρυψης που επιτρέπουν την προσαρμογή της διαδικασίας απόκρυψης."
type: docs
weight: 430
url: /el/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Αντιπροσωπεύει τις ρυθμίσεις διαγραφής, επιτρέποντας την προσαρμογή της διαδικασίας διαγραφής.

```csharp
public class RedactorSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο ILogger. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IOcrConnector. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings με ένα δεδομένο αντικείμενο IRedactionCallback. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger και IRedactionCallback. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactorSettings με δεδομένα αντικείμενα ILogger, IRedactionCallback και IOcrConnector. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Λαμβάνει ή ορίζει ένα αντικείμενο κλάσης, που υλοποιεί [`ILogger`](../ilogger), το οποίο χρησιμοποιείται για την καταγραφή συμβάντων και σφαλμάτων. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | Λαμβάνει ή ορίζει ένα αντικείμενο κλάσης, που υλοποιεί το interface [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector). |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | Λαμβάνει ή ορίζει ένα αντικείμενο κλάσης, που υλοποιεί το [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback). |

### Παρατηρήσεις

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
