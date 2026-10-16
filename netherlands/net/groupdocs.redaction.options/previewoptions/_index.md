---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt opties om vereisten en streamdelegaten in te stellen voor het genereren van een voorbeeld."
type: docs
weight: 400
url: /nl/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Biedt opties om vereisten en streamdelegaten in te stellen voor het genereren van een voorbeeld.

```csharp
public class PreviewOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Initialiseert een nieuwe instantie van de klasse PreviewOptions, waardoor de uitvoerstroom wordt gesloten. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Initialiseert een nieuwe instantie van de klasse PreviewOptions, waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Haalt op of stelt een instantie van de paginastroom‑creatie‑delegate in. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Haalt op of stelt de hoogte van de paginavoorvertoning in. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Haalt op of stelt een array met paginanummers in om een voorvertoning te genereren. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Haalt op of stelt het formaat van de voorvertoningsafbeelding in. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Haalt op of stelt een instantie van de paginavoorvertonings‑voltooiings‑delegate in. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Haalt op of stelt de breedte van de paginavoorvertoning in. |

### Voorbeelden

Het volgende voorbeeld toont hoe een documentvoorvertoning te verkrijgen met behulp van [`PreviewOptions`](../previewoptions) en de [`CreatePageStream`](./createpagestream)‑delegate.

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
