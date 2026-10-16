---
title: "ReleasePageStream"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une méthode qui libère le flux créé par le délégué CreatePageStream./createpagestream."
type: docs
weight: 440
url: /fr/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Représente une méthode qui libère le flux créé par le délégué [`CreatePageStream`](../createpagestream).

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageNumber | Int32 | Numéro de page de l'aperçu de page généré |
| pageStream | Stream | Flux contenant l'aperçu de page généré |

### Exemples

L'exemple suivant montre comment obtenir un aperçu de document en utilisant [`PreviewOptions`](../previewoptions) et les deux délégués.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // faire n'importe quoi avec le Stream contenant l'aperçu de page
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

### Voir aussi

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
