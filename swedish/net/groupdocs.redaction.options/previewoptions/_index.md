---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller alternativ för att ange krav och strömsdelegeringar för generering av förhandsgranskning."
type: docs
weight: 400
url: /sv/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Tillhandahåller alternativ för att ange krav och strömsdelegeringar för generering av förhandsgranskning.

```csharp
public class PreviewOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Initierar en ny instans av PreviewOptions-klassen, vilket får utdataströmmen att stängas. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Initierar en ny instans av PreviewOptions-klassen, vilket får utdataströmmen att returneras till klienten för vidare användning. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Hämtar eller anger en instans av sidströmsskapande delegat. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Hämtar eller anger sidförhandsgranskningshöjd. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Hämtar eller anger en array av sidnummer för att generera förhandsgranskning. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Hämtar eller anger format för förhandsgranskningsbild. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Hämtar eller anger en instans av delegat för slutförande av sidförhandsgranskning. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Hämtar eller anger sidförhandsgranskningsbredd. |

### Exempel

Följande exempel visar hur man får en dokumentförhandsgranskning med hjälp av [`PreviewOptions`](../previewoptions) och delegaten [`CreatePageStream`](./createpagestream).

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

Följande exempel visar hur man får en dokumentförhandsgranskning med hjälp av [`PreviewOptions`](../previewoptions) och båda delegaterna.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // gör vad som helst med Stream, som innehåller sidförhandsgranskning
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

### Se även

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
