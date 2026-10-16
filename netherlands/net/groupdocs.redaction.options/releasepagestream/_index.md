---
title: "ReleasePageStream"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een methode voor die de door CreatePageStream./createpagestream gemaakte stream vrijgeeft."
type: docs
weight: 440
url: /nl/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Stelt een methode voor die de door [`CreatePageStream`](../createpagestream) gemaakte stream vrijgeeft.

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageNumber | Int32 | Paginanummer van de gegenereerde paginavoorbeeld |
| pageStream | Stream | Stream, met de gegenereerde paginavoorbeeld |

### Voorbeelden

Het volgende voorbeeld toont hoe een documentvoorvertoning te verkrijgen met behulp van [`PreviewOptions`](../previewoptions) en beide delegates.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // Doe alles met Stream, die een paginavoorvertoning bevat
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

### Zie ook

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
