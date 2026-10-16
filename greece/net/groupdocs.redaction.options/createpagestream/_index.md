---
title: "CreatePageStream"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει τη μέθοδο που επιστρέφει ένα stream για την εγγραφή δεδομένων προεπισκόπησης σελίδας."
type: docs
weight: 300
url: /el/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Αντιπροσωπεύει τη μέθοδο που επιστρέφει ένα stream για την εγγραφή δεδομένων προεπισκόπησης σελίδας.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageNumber | Int32 | Αριθμός σελίδας μιας σελίδας για δημιουργία μικρογραφίας |

### Τιμή Επιστροφής

Ροή για εγγραφή προεπισκόπησης σελίδας

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας τον εκχωρητή [`PreviewOptions`](../previewoptions) και [`CreatePageStream`](../createpagestream).

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

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
