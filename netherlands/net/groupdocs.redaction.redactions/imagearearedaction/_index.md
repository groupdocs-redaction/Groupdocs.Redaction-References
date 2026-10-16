---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een redactie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een afbeeldingsdocument."
type: docs
weight: 630
url: /nl/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Stelt een redactie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een afbeeldingsdocument.

```csharp
public class ImageAreaRedaction : Redaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Initialiseert een nieuw exemplaar van de ImageAreaRedaction-klasse voor het redigeren van een specifieke gebiedsgrootte. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Haalt de [`RegionReplacementOptions`](../regionreplacementoptions) opties op met kleur- en gebiedsparameters. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Haalt de linkerbovenpositie van het te verwijderen gebied op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
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

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
