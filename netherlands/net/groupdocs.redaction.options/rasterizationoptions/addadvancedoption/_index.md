---
title: AddAdvancedOption
second_title: GroupDocs.Redaction voor .NET API-referentie
description: U kunt deze methode gebruiken om een geavanceerde rasteringsoptie te registreren om toe te passen.
type: docs
weight: 70
url: /nl/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

U kunt deze methode gebruiken om een geavanceerde rasteringsoptie te registreren om toe te passen.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Geeft informatie over het geselecteerde effecttype (grijstinten, rand, etc.) |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u de geavanceerde rasteropties met standaardinstellingen toepast.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met standaardopties (pagina's converteren naar afbeeldingen, opslaan als PDF)
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
* naamruimte [GroupDocs.Redaction.Options](../../rasterizationoptions)
* montage [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

U kunt deze methode gebruiken om een geavanceerde rasteringsoptie te registreren om toe te passen.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Geeft informatie over het geselecteerde effecttype (grijstinten, rand, etc.) |
| parameters | Dictionary`2 | Parameters voor het gegeven effect, zoals rotatiehoek |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u de geavanceerde rasteropties met standaardinstellingen toepast.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met standaardopties (pagina's converteren naar afbeeldingen, opslaan als PDF)
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

Het volgende voorbeeld laat zien hoe u de geavanceerde rasteringoptie voor randen met aangepaste instellingen toepast.

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

Het volgende voorbeeld laat zien hoe u de optie voor geavanceerde rastering met ruis toepast met aangepaste instellingen.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met het aangepaste aantal en de grootte van ruiseffecten
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

In het volgende voorbeeld ziet u hoe u de optie Tilt geavanceerde rastering met aangepaste instellingen toepast.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Sla het document op met het aangepaste kanteleffect
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
* naamruimte [GroupDocs.Redaction.Options](../../rasterizationoptions)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
