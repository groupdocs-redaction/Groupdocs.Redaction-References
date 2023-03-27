---
title: RasterizationOptions
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Biedt opties voor het converteren van bestanden naar PDF.
type: docs
weight: 350
url: /nl/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Biedt opties voor het converteren van bestanden naar PDF.

```csharp
public class RasterizationOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialiseert een nieuwe instantie. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Haalt of stelt het PDF-nalevingsniveau in. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. TRUE standaard ingesteld op FALSE om rastering te voorkomen. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Krijgt een indicator, wat waar is als geavanceerde rasteropties zijn ingesteld. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Haalt of stelt het aantal pagina's in dat moet worden geconverteerd naar PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Haalt of stelt de index van de eerste pagina in (0-gebaseerd) om te converteren naar PDF. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | U kunt deze methode gebruiken om een geavanceerde rasteringsoptie te registreren om toe te passen. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | U kunt deze methode gebruiken om een geavanceerde rasteringsoptie te registreren om toe te passen. |

### Opmerkingen

**Kom meer te weten**

* Meer informatie over het opslaan van documenten als een gerasterde PDF: [Opslaan in gerasterde PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Meer details over opties voor rasteren: [Selecteer specifieke pagina's voor gerasterde PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe u opties instelt voor het rasterisatieproces.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // verwerk gevoelige gegevens op de eerste dia 
    
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

* naamruimte [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
