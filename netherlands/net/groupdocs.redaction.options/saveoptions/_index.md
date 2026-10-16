---
title: "SaveOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt opties voor het wijzigen van een uitvoerbestandsnaam en/of het converteren van het document naar op afbeeldingen gebaseerde PDF-rasterisatie."
type: docs
weight: 450
url: /nl/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Biedt opties om de naam van een uitvoerbestand te wijzigen en/of het document te converteren naar een op afbeeldingen gebaseerde PDF (rasterisatie).

```csharp
public class SaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Initialiseert een nieuw exemplaar met standaardwaarden: rasteren naar PDF - false, suffix toevoegen - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Initialiseert een nieuw exemplaar met opgegeven parameters. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard false. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Haalt de rasterisatie-instellingen op. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Haalt op of stelt een waarde in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Haalt op of stelt een aangepaste suffix in voor de uitvoerbestandsnaam. Als deze niet is opgegeven, wordt de [`SaveSuffix`](./savesuffix) constante gebruikt. |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Haalt de opslagopties op die specifiek zijn voor tekstverwerkingsdocumenten. |

## Velden

| Naam | Beschrijving |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Stelt de standaard suffixwaarde voor, die \"Redacted\" is. |

### Opmerkingen

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe een document op te slaan met SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Documentredactie komt hier
       // ...
    
       // Sla het document op met standaardopties (converteer pagina's naar afbeeldingen, sla op als PDF)
       redactor.Save();
    
       // Sla het document op in het oorspronkelijke formaat en overschrijf het originele bestand
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Sla het document op naar een \"*_Redacted.*\" bestand in het oorspronkelijke formaat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Sla het document op naar \"*_AnyText.*\" (bijv. tijdstempel in plaats van \"AnyText\") in de bestandsnaam zonder rasterisatie
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Zie ook

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
