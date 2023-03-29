---
title: CreatePageStream
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt de methode die een stream retourneert om paginavoorbeeldgegevens te schrijven.
type: docs
weight: 290
url: /nl/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Vertegenwoordigt de methode die een stream retourneert om paginavoorbeeldgegevens te schrijven.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageNumber | Int32 | Paginanummer van een pagina om miniatuur te genereren |

### Winstwaarde

Stream om paginavoorbeeld te schrijven

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een documentvoorbeeld krijgt met behulp van[`PreviewOptions`](../previewoptions) En[`CreatePageStream`](../createpagestream) delegeren.

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

* naamruimte [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->