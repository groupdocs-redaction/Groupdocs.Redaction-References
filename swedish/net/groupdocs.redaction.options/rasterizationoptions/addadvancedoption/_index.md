---
title: AddAdvancedOption
second_title: GroupDocs.Redaction för .NET API-referens
description: Du kan använda den här metoden för att registrera ett avancerat rastreringsalternativ att tillämpa.
type: docs
weight: 70
url: /sv/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Du kan använda den här metoden för att registrera ett avancerat rastreringsalternativ att tillämpa.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Ger information om den valda effekttypen (gråskala, ram, etc.) |

### Exempel

Följande exempel visar hur du tillämpar de avancerade rastreringsalternativen med standardinställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med standardalternativ (konvertera sidor till bilder, spara som PDF)
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

### Se även

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namnutrymme [GroupDocs.Redaction.Options](../../rasterizationoptions)
* hopsättning [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Du kan använda den här metoden för att registrera ett avancerat rastreringsalternativ att tillämpa.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Ger information om den valda effekttypen (gråskala, ram, etc.) |
| parameters | Dictionary`2 | Parametrar för den givna effekten, såsom rotationsvinkel |

### Exempel

Följande exempel visar hur du tillämpar de avancerade rastreringsalternativen med standardinställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med standardalternativ (konvertera sidor till bilder, spara som PDF)
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

Följande exempel visar hur man använder det avancerade rastreringsalternativet för kantgränser med anpassade inställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med en anpassad ram
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Följande exempel visar hur du använder det avancerade brusrasteriseringsalternativet med anpassade inställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med anpassat antal och storlek på bruseffekter
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Följande exempel visar hur du använder det avancerade rastreringsalternativet för tilt med anpassade inställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med den anpassade lutningseffekten
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Se även

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namnutrymme [GroupDocs.Redaction.Options](../../rasterizationoptions)
* hopsättning [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
