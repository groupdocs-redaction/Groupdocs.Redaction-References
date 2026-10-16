---
title: "AddAdvancedOption"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "U kunt deze methode gebruiken om een geavanceerde rasterisatie‑optie te registreren die moet worden toegepast."
type: docs
weight: 70
url: /nl/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

U kunt deze methode gebruiken om een geavanceerde rasterisatie‑optie te registreren die moet worden toegepast.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |

### Voorbeelden

Het volgende voorbeeld laat zien hoe de geavanceerde rasterisatie-opties toe te passen met standaardinstellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met standaardopties (converteer pagina's naar afbeeldingen, sla op als PDF)
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

### Zie ook

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

U kunt deze methode gebruiken om een geavanceerde rasterisatie‑optie te registreren die moet worden toegepast.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |
| parameters | Dictionary`2 | Parameters voor het opgegeven effect, zoals rotatiehoek. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe de geavanceerde rasterisatie-opties toe te passen met standaardinstellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met standaardopties (converteer pagina's naar afbeeldingen, sla op als PDF)
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

Het volgende voorbeeld laat zien hoe de geavanceerde rasterisatie-optie voor randen toe te passen met aangepaste instellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met een aangepaste rand
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Het volgende voorbeeld laat zien hoe de geavanceerde rasterisatie-optie voor ruis toe te passen met aangepaste instellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met het aangepaste aantal en de grootte van ruis-effecten
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Het volgende voorbeeld toont hoe de geavanceerde rasterisatie-optie 'tilt' toe te passen met aangepaste instellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met het aangepaste tilt-effect
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Zie ook

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
