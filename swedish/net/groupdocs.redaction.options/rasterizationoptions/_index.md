---
title: RasterizationOptions
second_title: GroupDocs.Redaction för .NET API-referens
description: Ger alternativ för att konvertera filer till PDF.
type: docs
weight: 350
url: /sv/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Ger alternativ för att konvertera filer till PDF.

```csharp
public class RasterizationOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initierar en ny instans. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Hämtar eller ställer in PDF-efterlevnadsnivån. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Hämtar eller ställer in ett värde som anger om alla sidor i dokumentet behöver konverteras till bilder och läggas i en enda PDF-fil. TRUE som standard, inställt på FALSE för att undvika rastrering. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Får en indikator, vilket är sant om avancerade rastreringsalternativ är inställda. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska konverteras till PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Hämtar eller ställer in indexet för den första sidan (0-baserad) som ska konverteras till PDF. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Du kan använda den här metoden för att registrera ett avancerat rastreringsalternativ att tillämpa. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Du kan använda den här metoden för att registrera ett avancerat rastreringsalternativ att tillämpa. |

### Anmärkningar

**Läs mer**

* Mer information om att spara dokument som en rastrerad PDF: [Spara i rastrerad PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Mer information om rastreringsalternativ: [Välj specifika sidor för rastrerad PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Exempel

Följande exempel visar hur du ställer in alternativ för rastreringsprocessen.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // redigera känslig data på den första bilden 
    
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

* namnutrymme [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
