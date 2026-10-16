---
title: "AdvancedRasterizationOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Énumération de drapeaux pour gérer les options avancées de rasterisation à appliquer."
type: docs
weight: 290
url: /fr/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Énumération de drapeaux pour gérer les options avancées de rasterisation à appliquer.

```csharp
public enum AdvancedRasterizationOptions
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune option avancée à appliquer. |
| Tilt | `1` | Inclinez l'image rasterisée à un angle aléatoire. |
| Noise | `2` | Ajoutez des taches aléatoires aux images de pages rasterisées. |
| Border | `4` | Ajoutez une bordure pour imiter l'effet de numérisation de page. |
| Grayscale | `8` | Rendez les images de pages en niveaux de gris pour imiter une numérisation en niveaux de gris. |

### Exemples

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
