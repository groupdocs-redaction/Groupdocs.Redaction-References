---
title: "DocumentFormatConfiguration"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια αναφορά τύπου για την κλάση DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived και τη λίστα των υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερη ανίχνευση μορφής."
type: docs
weight: 10
url: /el/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Αντιπροσωπεύει μια αναφορά τύπου για κλάση προεξαίρεσης από [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) και λίστα των υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερη ανίχνευση μορφής.

```csharp
public class DocumentFormatConfiguration
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Αρχικοποιεί μια νέα παρουσία της κλάσης DocumentFormatConfiguration. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Λαμβάνει ή ορίζει τον τύπο μιας κλάσης, η οποία κληρονομεί από [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Λαμβάνει ή ορίζει μια λίστα επεκτάσεων αρχείων διαχωρισμένη με κόμμα (\",\") (π.χ. \".pdf\"), χωρίς διάκριση πεζών-κεφαλαίων. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Λαμβάνει ή ορίζει δεδομένα, απαιτούμενα για την αρχικοποίηση του [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Ελέγχει εάν μια δεδομένη επέκταση αρχείου μπορεί να αντιμετωπιστεί ως DocumentType. |

### Παρατηρήσεις

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ορίσετε ιδιότητες για μια προσαρμοσμένη διαμόρφωση μορφής.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
