---
title: "RasterizationOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des options pour convertir des fichiers en PDF."
type: docs
weight: 420
url: /fr/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Fournit des options pour convertir des fichiers en PDF.

```csharp
public class RasterizationOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialise une nouvelle instance. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Obtient ou définit le niveau de conformité PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Obtient ou définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, définissez sur FALSE pour éviter la rasterisation. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Obtient un indicateur, qui est true si des options de rasterisation avancées sont définies. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à convertir en PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Obtient ou définit l’index de la première page (0-based) à convertir en PDF. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer. |

### Remarques

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Exemples

L’exemple suivant montre comment définir les options pour le processus de rasterisation.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // masquer les données sensibles sur la première diapositive 
    
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

L'exemple suivant montre comment appliquer les options de rasterisation avancées avec les paramètres par défaut.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistrez le document avec les options par défaut (convertir les pages en images, enregistrer en PDF)
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

L'exemple suivant montre comment appliquer l'option de rasterisation avancée de bordure avec des paramètres personnalisés.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistrez le document avec une bordure personnalisée
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

L'exemple suivant montre comment appliquer l'option de rasterisation avancée de bruit avec des paramètres personnalisés.

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

L'exemple suivant montre comment appliquer l'option de rastérisation avancée tilt avec des paramètres personnalisés.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Enregistrez le document avec l'effet tilt personnalisé
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Voir aussi

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
