---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en redigering som placerar en färgad rektangel i ett givet område av ett bilddokument."
type: docs
weight: 630
url: /sv/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Representerar en redigering som placerar en färgad rektangel i ett givet område av ett bilddokument.

```csharp
public class ImageAreaRedaction : Redaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Initierar en ny instans av ImageAreaRedaction-klassen för att radera en specifik områdesstorlek. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Hämtar [`RegionReplacementOptions`](../regionreplacementoptions)-alternativen med färg- och områdesparametrar. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Hämtar den övre vänstra positionen för området som ska tas bort |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
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

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
