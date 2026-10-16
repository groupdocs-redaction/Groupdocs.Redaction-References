---
title: "GeneratePreview"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Génère des images d'aperçu de pages spécifiques dans un format d'image donné."
type: docs
weight: 40
url: /fr/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

Génère des images d'aperçu de pages spécifiques dans un format d'image donné.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| previewOptions | PreviewOptions | Paramètres des propriétés d'image et de la plage de pages |

### Exemples

L'exemple suivant montre comment obtenir un aperçu du document en utilisant [`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions) et les deux délégués.

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

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
