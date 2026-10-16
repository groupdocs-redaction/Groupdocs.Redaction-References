---
title: "GeneratePreview"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας."
type: docs
weight: 40
url: /el/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| previewOptions | PreviewOptions | Ιδιότητες εικόνας και ρυθμίσεις εύρους σελίδων |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε μια προεπισκόπηση εγγράφου χρησιμοποιώντας το [`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions) και τους δύο αντιπροσώπους.

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

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
