---
title: "CreatePageStream"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une méthode qui renvoie un flux pour écrire les données d'aperçu de page."
type: docs
weight: 300
url: /fr/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Représente une méthode qui renvoie un flux pour écrire les données d'aperçu de page.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageNumber | Int32 | Numéro de page d'une page pour générer la miniature |

### Valeur de retour

Flux pour écrire l'aperçu de page

### Exemples

L'exemple suivant montre comment obtenir un aperçu du document en utilisant le délégué [`PreviewOptions`](../previewoptions) et [`CreatePageStream`](../createpagestream).

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

### Voir aussi

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
