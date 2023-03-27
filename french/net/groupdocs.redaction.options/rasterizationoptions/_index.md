---
title: RasterizationOptions
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Fournit des options pour convertir des fichiers en PDF.
type: docs
weight: 350
url: /fr/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Fournit des options pour convertir des fichiers en PDF.

```csharp
public class RasterizationOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialise une nouvelle instance. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Obtient ou définit le niveau de conformité PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Obtient ou définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, défini sur FALSE afin d'éviter la pixellisation. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Obtient un indicateur, qui est vrai si les options de pixellisation avancées sont définies. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à convertir en PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Obtient ou définit l'index de la première page (base 0) à convertir en PDF. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Vous pouvez utiliser cette méthode pour enregistrer une option de pixellisation avancée à appliquer. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Vous pouvez utiliser cette méthode pour enregistrer une option de pixellisation avancée à appliquer. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'enregistrement d'un document au format PDF pixellisé : [Enregistrer au format PDF pixellisé](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Plus de détails sur les options de pixellisation : [Sélectionnez des pages spécifiques pour le PDF pixellisé](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Exemples

L'exemple suivant montre comment définir des options pour le processus de pixellisation.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // expurger les données sensibles sur la première diapositive 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

L'exemple suivant montre comment appliquer les options de pixellisation avancées avec les paramètres par défaut.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistrer le document avec les options par défaut (convertir les pages en images, enregistrer au format PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

L'exemple suivant montre comment appliquer l'option de pixellisation avancée des bordures avec des paramètres personnalisés.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistre le document avec une bordure personnalisée
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

L'exemple suivant montre comment appliquer l'option de pixellisation avancée du bruit avec des paramètres personnalisés.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistrez le document avec le nombre et la taille personnalisés des effets de bruit
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

L'exemple suivant montre comment appliquer l'option de pixellisation avancée d'inclinaison avec des paramètres personnalisés.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistre le document avec l'effet d'inclinaison personnalisé
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Voir également

* espace de noms [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
