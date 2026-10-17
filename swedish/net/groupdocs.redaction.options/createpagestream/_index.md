---
title: "CreatePageStream"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en metod som returnerar en ström för att skriva data för sidförhandsgranskning."
type: docs
weight: 300
url: /sv/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Representerar en metod som returnerar en ström för att skriva data för sidförhandsgranskning.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageNumber | Int32 | Sidnummer för en sida som ska generera en miniatyrbild |

### Returvärde

Ström för att skriva sidförhandsgranskning

### Exempel

Följande exempel visar hur man får en dokumentförhandsgranskning med hjälp av [`PreviewOptions`](../previewoptions) och [`CreatePageStream`](../createpagestream)-delegaten.

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
