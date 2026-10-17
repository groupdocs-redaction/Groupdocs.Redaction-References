---
title: "Punkt"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Identifierar en pixeloffset på en sida eller bild, vanligtvis det övre vänstra hörnet av ett redigeringsområde."
type: docs
weight: 340
url: /sv/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Identifierar en pixeloffset på en sida eller bild, vanligtvis det övre vänstra hörnet av ett redigeringsområde.

```csharp
public struct Point : IEquatable<Point>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Point](point)(int, int) | Skapar en punkt för ursprunget av ett redigeringsområde. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | En punkt vid ursprunget (0, 0). |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Horisontell offset från vänster kant, i pixlar. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Vertikal offset från övre kant, i pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Jämför denna punkt med ett annat objekt. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Jämför koordinater med en annan punkt. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Returnerar en hashkod härledd från koordinaterna. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Returnerar koordinaterna i ett läsbart format. |

### Se även

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
