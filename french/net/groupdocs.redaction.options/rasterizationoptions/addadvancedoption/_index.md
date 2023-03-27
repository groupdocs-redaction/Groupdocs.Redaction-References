---
title: AddAdvancedOption
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Vous pouvez utiliser cette méthode pour enregistrer une option de pixellisation avancée à appliquer.
type: docs
weight: 70
url: /fr/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Vous pouvez utiliser cette méthode pour enregistrer une option de pixellisation avancée à appliquer.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |

### Exemples

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

### Voir également

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* espace de noms [GroupDocs.Redaction.Options](../../rasterizationoptions)
* Assemblée [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Vous pouvez utiliser cette méthode pour enregistrer une option de pixellisation avancée à appliquer.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |
| parameters | Dictionary`2 | Paramètres de l'effet donné, tels que l'angle de rotation |

### Exemples

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* espace de noms [GroupDocs.Redaction.Options](../../rasterizationoptions)
* Assemblée [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
