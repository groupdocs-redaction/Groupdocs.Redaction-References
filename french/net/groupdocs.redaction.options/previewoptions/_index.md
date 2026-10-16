---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus."
type: docs
weight: 400
url: /fr/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus.

```csharp
public class PreviewOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Initialise une nouvelle instance de la classe PreviewOptions, entraînant la fermeture du flux de sortie. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Initialise une nouvelle instance de la classe PreviewOptions, entraînant le renvoi du flux de sortie au client pour une utilisation ultérieure. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Obtient ou définit une instance du délégué de création de flux de page. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Obtient ou définit la hauteur de l'aperçu de page. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Obtient ou définit un tableau de numéros de page pour générer l'aperçu. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Obtient ou définit le format d'image d'aperçu. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Obtient ou définit une instance du délégué de fin d'aperçu de page. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Obtient ou définit la largeur de l'aperçu de page. |

### Exemples

L'exemple suivant montre comment obtenir un aperçu de document en utilisant le délégué [`PreviewOptions`](../previewoptions) et [`CreatePageStream`](./createpagestream).

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
