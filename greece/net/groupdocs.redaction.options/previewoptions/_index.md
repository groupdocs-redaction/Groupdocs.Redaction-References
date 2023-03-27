---
title: PreviewOptions
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Παρέχει επιλογές για ορισμό απαιτήσεων και ροή εκπροσώπων για δημιουργία προεπισκόπησης.
type: docs
weight: 330
url: /el/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Παρέχει επιλογές για ορισμό απαιτήσεων και ροή εκπροσώπων για δημιουργία προεπισκόπησης.

```csharp
public class PreviewOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Αρχικοποιεί μια νέα παρουσία της κλάσης PreviewOptions, προκαλώντας το κλείσιμο της ροής εξόδου. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Αρχικοποιεί μια νέα παρουσία της κλάσης PreviewOptions, με αποτέλεσμα η ροή εξόδου να επιστραφεί στον πελάτη για περαιτέρω χρήση. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του εκπροσώπου δημιουργίας ροής σελίδας. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Λαμβάνει ή ορίζει ύψος προεπισκόπησης σελίδας. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Λαμβάνει ή ορίζει μια σειρά από αριθμούς σελίδων για τη δημιουργία προεπισκόπησης. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του πληρεξούσιου ολοκλήρωσης προεπισκόπησης σελίδας. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Λαμβάνει ή ορίζει πλάτος προεπισκόπησης σελίδας. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να αποκτήσετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας[`PreviewOptions`](../previewoptions) και[`CreatePageStream`](./createpagestream) αντιπρόσωπος.

Το ακόλουθο παράδειγμα δείχνει πώς να αποκτήσετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας[`PreviewOptions`](../previewoptions) και των δύο αντιπροσώπων.

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

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // κάντε οτιδήποτε με το Stream, που περιέχει προεπισκόπηση σελίδας
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

* χώρος ονομάτων [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->