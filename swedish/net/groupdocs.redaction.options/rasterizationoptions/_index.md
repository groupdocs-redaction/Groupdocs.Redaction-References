---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller alternativ för att konvertera filer till PDF."
type: docs
weight: 420
url: /sv/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Tillhandahåller alternativ för att konvertera filer till PDF.

```csharp
public class RasterizationOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initierar en ny instans. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Hämtar eller anger PDF-efterlevnadsnivån. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Hämtar eller anger ett värde som indikerar om alla sidor i dokumentet ska konverteras till bilder och placeras i en enda PDF-fil. SANT som standard, sätt till FALSKT för att undvika rasterisering. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Hämtar en indikator som är sann om avancerade rasteriseringsalternativ är inställda. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Hämtar eller anger antalet sidor som ska konverteras till PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Hämtar eller anger indexet för den första sidan (0-baserat) som ska konverteras till PDF. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa. |

### Anmärkningar

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Exempel

Följande exempel visar hur man ställer in alternativ för rasteriseringsprocessen.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // radera känslig data på den första bilden 
    
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
