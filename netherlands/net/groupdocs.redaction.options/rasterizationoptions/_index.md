---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt opties voor het converteren van bestanden naar PDF."
type: docs
weight: 420
url: /nl/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Biedt opties voor het converteren van bestanden naar PDF.

```csharp
public class RasterizationOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialiseert een nieuw exemplaar. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Haalt het PDF‑compliance‑niveau op of stelt het in. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF‑bestand moeten worden geplaatst. Standaard WAAR, stel in op ONWAAR om rasterisatie te voorkomen. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Haalt een indicator op die WAAR is als geavanceerde rasterisatie‑opties zijn ingesteld. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Haalt het aantal pagina's op of stelt het in dat moet worden geconverteerd naar PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Haalt de index van de eerste pagina (0‑gebaseerd) op of stelt deze in om te converteren naar PDF. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | U kunt deze methode gebruiken om een geavanceerde rasterisatie‑optie te registreren die moet worden toegepast. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | U kunt deze methode gebruiken om een geavanceerde rasterisatie‑optie te registreren die moet worden toegepast. |

### Opmerkingen

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Voorbeelden

Het volgende voorbeeld toont hoe opties voor het rasterisatieproces kunnen worden ingesteld.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // redigeer gevoelige gegevens op de eerste dia 
    
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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
