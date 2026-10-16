---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt kleur‑ en gebiedsparameters voor vervanging van een afbeeldingsgebied voor. Zie ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /nl/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Stelt kleur‑ en gebiedsparameters voor vervanging van een afbeeldingsgebied voor. Zie [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Initialiseert een nieuwe instantie van de klasse RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Initialiseert een nieuwe instantie van de klasse RegionReplacementOptions waarvan de grootte overeenkomt met de opgegeven tekst. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Haalt op of stelt de kleur in om het geredigeerde gebied te vullen. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Haalt op of stelt de rechthoek met breedte en hoogte in. |

### Opmerkingen

**Learn more**

* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Voorbeelden

Het volgende voorbeeld toont het vervangen van een gebied binnen de afbeelding door een rechthoek met een effen kleur.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       GroupDocs.Redaction.Options.Drawing.Point samplePoint = new GroupDocs.Redaction.Options.Drawing.Point(516, 311);
       GroupDocs.Redaction.Options.Drawing.Size sampleSize = new GroupDocs.Redaction.Options.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Zie ook

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
