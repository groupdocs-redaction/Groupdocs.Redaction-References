---
title: "DocumentFormatInstance"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια συγκεκριμένη μορφή εγγράφου. Υλοποιήστε αυτήν την κλάση για να προσθέσετε τους δικούς σας τύπους εγγράφων."
type: docs
weight: 110
url: /el/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Αντιπροσωπεύει μια συγκεκριμένη μορφή εγγράφου. Υλοποιήστε αυτήν την κλάση για να προσθέσετε τους δικούς σας τύπους εγγράφων.

```csharp
public abstract class DocumentFormatInstance
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για έγγραφα προστατευμένα με κωδικό. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Εκτελεί την αρχικοποίηση του αντικειμένου διαχειριστή μορφής εγγράφου. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Ελέγχει για υλοποίηση του [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) και την καλεί, εάν έχει καθοριστεί. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Φορτώνει το έγγραφο από μια ροή. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Ελέγχει εάν η δοθείσα ροή περιέχει ένα έγγραφο, που υποστηρίζεται από αυτήν την παρουσία μορφής. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Αποθηκεύει το έγγραφο σε μια ροή. |

### Παρατηρήσεις

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να δημιουργήσετε ένα κενό stub για έναν προσαρμοσμένο διαχειριστή μορφής.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // φόρτωση περιεχομένου αρχείου
    }

    public override void Save(Stream output)
    {
        // αποθήκευση αλλαγών στο αρχείο;
    }
}
```

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

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
