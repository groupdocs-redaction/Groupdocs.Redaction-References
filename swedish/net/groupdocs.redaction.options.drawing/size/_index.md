---
title: "Storlek"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Definierar bredden och höjden på ett redigeringsområde i pixlar."
type: docs
weight: 360
url: /sv/net/groupdocs.redaction.options.drawing/size/
---
## Size structure

Definierar bredden och höjden på ett redigeringsområde i pixlar.

```csharp
public struct Size : IEquatable<Size>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Size](size)(int, int) | Skapar en storlek för ett rektangulärt raderingsområde. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/size/empty) { get; } | En noll bredd och höjd. |
| [Height](../../groupdocs.redaction.options.drawing/size/height) { get; } | Regionens höjd i pixlar. |
| [Width](../../groupdocs.redaction.options.drawing/size/width) { get; } | Regionens bredd i pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/size/equals#equals_1)(object) | Jämför den här storleken med ett annat objekt. |
| [Equals](../../groupdocs.redaction.options.drawing/size/equals#equals)(Size) | Jämför dimensioner med en annan storlek. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/size/gethashcode)() | Returnerar en hashkod härledd från bredd och höjd. |
| override [ToString](../../groupdocs.redaction.options.drawing/size/tostring)() | Returnerar dimensionerna i ett läsbart format. |

### Se även

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
