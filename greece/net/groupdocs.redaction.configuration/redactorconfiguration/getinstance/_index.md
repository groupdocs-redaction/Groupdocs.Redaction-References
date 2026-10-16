---
title: "GetInstance"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει μια μοναδική (singleton) παρουσία με προεπιλεγμένη διαμόρφωση των ενσωματωμένων μορφών."
type: docs
weight: 10
url: /el/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Παρέχει μια μοναδική παρουσία με προεπιλεγμένη διαμόρφωση των ενσωματωμένων μορφών.

```csharp
public static RedactorConfiguration GetInstance()
```

### Τιμή Επιστροφής

Παράδειγμα διαμόρφωσης

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να προσθέσετε έναν προσαρμοσμένο διαχειριστή μορφής.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Δείτε επίσης

* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
