---
title: CreatePageStream
second_title: GroupDocs.Redaction för .NET API-referens
description: Representerar en metod som returnerar en ström för att skriva sidförhandsgranskningsdata.
type: docs
weight: 280
url: /sv/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Representerar en metod som returnerar en ström för att skriva sidförhandsgranskningsdata.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageNumber | Int32 | Sidnummer för en sida för att generera miniatyrbild |

### Returvärde

Streama för att skriva förhandsgranskning av sidan

### Exempel

Följande exempel visar hur man får en förhandsgranskning av ett dokument med hjälp av[`PreviewOptions`](../previewoptions) och[`CreatePageStream`](../createpagestream) delegera.

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

### Se även

* namnutrymme [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->