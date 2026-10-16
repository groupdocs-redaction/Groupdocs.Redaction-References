---
title: "GeneratePreview"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Genereert voorbeeldafbeeldingen van specifieke pagina's in een gegeven afbeeldingsformaat."
type: docs
weight: 40
url: /nl/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

Genereert voorbeeldafbeeldingen van specifieke pagina's in een gegeven afbeeldingsformaat.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| previewOptions | PreviewOptions | Afbeeldingseigenschappen en paginabereikinstellingen |

### Voorbeelden

Het volgende voorbeeld laat zien hoe een documentvoorbeeld te verkrijgen met behulp van [`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions) en beide delegaten.

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

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
