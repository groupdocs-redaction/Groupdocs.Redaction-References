---
title: "ReleasePageStream"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια μέθοδο που απελευθερώνει τη ροή που δημιουργήθηκε από τον εκχωρητή CreatePageStream./createpagestream."
type: docs
weight: 440
url: /el/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Αντιπροσωπεύει μια μέθοδο που απελευθερώνει τη ροή που δημιουργήθηκε από τον εκχωρητή [`CreatePageStream`](../createpagestream).

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageNumber | Int32 | Αριθμός σελίδας της παραγόμενης προεπισκόπησης σελίδας |
| pageStream | Stream | Ροή, που περιέχει την παραγόμενη προεπισκόπηση σελίδας |

### Παραδείγματα

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
