---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει πρόσβαση σε μια λίστα των υποστηριζόμενων μορφών ενσωματωμένων και προσαρμοσμένων μορφών χρήστη."
type: docs
weight: 20
url: /el/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Παρέχει πρόσβαση σε μια λίστα υποστηριζόμενων μορφών, ενσωματωμένων και προσαρμοσμένων μορφών χρήστη.

```csharp
public class RedactorConfiguration
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Λαμβάνει μια λίστα των αναγνωρισμένων μορφών, δείτε [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Παρέχει μια μοναδική παρουσία με προεπιλεγμένη διαμόρφωση των ενσωματωμένων μορφών. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Εντοπίζει τις διαμορφώσεις μορφής για μια δεδομένη επέκταση αρχείου. |

### Παρατηρήσεις

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να προσθέσετε έναν προσαρμοσμένο χειριστή μορφής χρήστη.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε ενσωματωμένους ή προσαρμοσμένους χειριστές μορφής χρήστη.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
