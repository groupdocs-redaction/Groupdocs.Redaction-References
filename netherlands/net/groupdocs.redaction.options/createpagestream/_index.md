---
title: "CreatePageStream"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een methode voor die een stream retourneert om paginavoorbeeldgegevens te schrijven."
type: docs
weight: 300
url: /nl/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Stelt een methode voor die een stream retourneert om paginavoorbeeldgegevens te schrijven.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageNumber | Int32 | Paginanummer van een pagina om een miniatuur te genereren |

### Retourwaarde

Stream om paginavoorbeeld te schrijven

### Voorbeelden

Het volgende voorbeeld toont hoe een documentvoorbeeld te verkrijgen met behulp van [`PreviewOptions`](../previewoptions) en [`CreatePageStream`](../createpagestream) delegate.

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

### Zie ook

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
