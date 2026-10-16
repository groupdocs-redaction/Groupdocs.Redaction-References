---
title: "FindFormat"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Εντοπίζει τις διαμορφώσεις μορφής για μια δεδομένη επέκταση αρχείου."
type: docs
weight: 30
url: /el/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Εντοπίζει τις διαμορφώσεις μορφής για μια δεδομένη επέκταση αρχείου.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileExtension | String | Επέκταση αρχείου, η μορφή είναι ".ext" |

### Τιμή Επιστροφής

Εάν βρεθεί, η παρουσία είναι του [`DocumentFormatConfiguration`](../../documentformatconfiguration), διαφορετικά null

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε ενσωματωμένους ή προσαρμοσμένους χειριστές μορφής χρήστη.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Δείτε επίσης

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
