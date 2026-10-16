---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει επιλογές για τον ορισμό απαιτήσεων και των delegates του stream για τη δημιουργία προεπισκόπησης."
type: docs
weight: 400
url: /el/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Παρέχει επιλογές για τον ορισμό απαιτήσεων και των delegates του stream για τη δημιουργία προεπισκόπησης.

```csharp
public class PreviewOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας το κλείσιμο της ροής εξόδου. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Λαμβάνει ή ορίζει ένα αντικείμενο του delegate δημιουργίας ροής σελίδας. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Λαμβάνει ή ορίζει το ύψος της προεπισκόπησης σελίδας. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Λαμβάνει ή ορίζει έναν πίνακα αριθμών σελίδων για τη δημιουργία προεπισκόπησης. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Λαμβάνει ή ορίζει ένα αντικείμενο του delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Λαμβάνει ή ορίζει το πλάτος της προεπισκόπησης σελίδας. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας το [`PreviewOptions`](../previewoptions) και το delegate [`CreatePageStream`](./createpagestream).

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    var previewOptions = new PreviewOptions(createDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας το [`PreviewOptions`](../previewoptions) και τους δύο delegates.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // κάντε οτιδήποτε με το Stream, που περιέχει την προεπισκόπηση σελίδας
        pageStream.Close();
    };
    var previewOptions = new PreviewOptions(createDelegate, releaseDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
