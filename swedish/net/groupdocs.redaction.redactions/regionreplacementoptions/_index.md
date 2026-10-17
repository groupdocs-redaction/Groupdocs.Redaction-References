---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar färg- och områdesparametrar för bildregionersättning. Se ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /sv/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Representerar färg- och områdesparametrar för bildregionersättning. Se [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Initierar en ny instans av klassen RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Initierar en ny instans av klassen RegionReplacementOptions vars storlek matchar given text. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Hämtar eller anger färgen för att fylla den redigerade ytan. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Hämtar eller anger rektangeln med bredd och höjd. |

### Anmärkningar

**Learn more**

* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Exempel

Följande exempel visar hur man ersätter ett område i bilden med en rektangel i en solid färg.

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

### Se även

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
