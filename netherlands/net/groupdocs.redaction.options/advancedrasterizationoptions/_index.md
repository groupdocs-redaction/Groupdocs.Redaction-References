---
title: "AdvancedRasterizationOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Vlaggenenumeratie om de geavanceerde rasterisatieopties te beheren die moeten worden toegepast."
type: docs
weight: 290
url: /nl/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Vlaggenenumeratie om de geavanceerde rasterisatieopties te beheren die moeten worden toegepast.

```csharp
public enum AdvancedRasterizationOptions
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Geen geavanceerde opties om toe te passen. |
| Tilt | `1` | Kantelen om de gerasterde afbeelding naar een willekeurige hoek te hellen. |
| Noise | `2` | Voeg willekeurige vlekken toe aan gerasterde paginabeelden. |
| Border | `4` | Voeg een randlijn toe om het effect van een paginascans na te bootsen. |
| Grayscale | `8` | Maak paginabeelden grijswaarden om een grijswaarden-scan na te bootsen. |

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
