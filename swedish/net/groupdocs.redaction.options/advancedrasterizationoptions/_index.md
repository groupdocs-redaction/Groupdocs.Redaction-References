---
title: "AdvancedRasterizationOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Flagg‑uppräkning för att hantera de avancerade rasteriseringsalternativen som ska tillämpas."
type: docs
weight: 290
url: /sv/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Flagg‑uppräkning för att hantera de avancerade rasteriseringsalternativen som ska tillämpas.

```csharp
public enum AdvancedRasterizationOptions
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inga avancerade alternativ att tillämpa. |
| Tilt | `1` | Luta för att vinkla den rasteriserade bilden till en slumpmässig vinkel. |
| Noise | `2` | Lägg till slumpmässiga fläckar på rasteriserade sidbilder. |
| Border | `4` | Lägg till en kantlinje för att efterlikna en sidskannings-effekt. |
| Grayscale | `8` | Gör sidbilder i gråskala för att efterlikna en gråskalaskanning. |

### Exempel

Följande exempel visar hur man tillämpar de avancerade rasteriseringsalternativen med standardinställningar.

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

Följande exempel visar hur man tillämpar det avancerade rasteriseringsalternativet för kant med anpassade inställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med en anpassad kant
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Följande exempel visar hur man tillämpar det avancerade rasteriseringsalternativet för brus med anpassade inställningar.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Spara dokumentet med det anpassade antalet och storleken på brus-effekter
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Följande exempel visar hur man tillämpar lutningsalternativet för avancerad rasterisering med anpassade inställningar.

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
