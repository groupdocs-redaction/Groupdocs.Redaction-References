---
title: ReleasePageStream
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une méthode qui libère le flux créé parCreatePageStream./createpagestream déléguer.
type: docs
weight: 360
url: /fr/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Représente une méthode qui libère le flux créé par[`CreatePageStream`](../createpagestream) déléguer.

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageNumber | Int32 | Numéro de page de l'aperçu de page généré |
| pageStream | Stream | Stream, contenant l'aperçu de la page générée |

### Exemples

L'exemple suivant montre comment obtenir un aperçu de document à l'aide de[`PreviewOptions`](../previewoptions) et les deux délégués.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // faire n'importe quoi avec Stream, contenant l'aperçu de la page
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

### Voir également

* espace de noms [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->