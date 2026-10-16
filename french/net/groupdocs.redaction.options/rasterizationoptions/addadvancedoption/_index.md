---
title: "AddAdvancedOption"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer."
type: docs
weight: 70
url: /fr/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |

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

### Voir aussi

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |
| paramètres | Dictionary`2 | Paramètres pour l'effet donné, tels que l'angle de rotation |

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
