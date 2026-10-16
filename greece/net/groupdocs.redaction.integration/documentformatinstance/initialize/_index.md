---
title: "Initialize"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Εκτελεί την αρχικοποίηση του αντικειμένου διαχειριστή μορφής εγγράφου."
type: docs
weight: 20
url: /el/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Εκτελεί την αρχικοποίηση του αντικειμένου διαχειριστή μορφής εγγράφου.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαμόρφωση | DocumentFormatConfiguration | Διαμόρφωση μορφής |
| ρυθμίσεις | RedactorSettings | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξεργασίας. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να χρησιμοποιήσετε τα δεδομένα αρχικοποίησης.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Άλλος προσαρμοσμένος κώδικας 
    ...

    public override void Initialize(DocumentFormatConfiguration config)
    {
        base.Initialize(config);
        if (config.InitializationData.ContainsKey("MyProperty"))
        {
            MyProperty = config.InitializationData["MyProperty"];
        }
    }
}

// Ενσωμάτωση προσαρμοσμένης μορφής στο GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Δείτε επίσης

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
