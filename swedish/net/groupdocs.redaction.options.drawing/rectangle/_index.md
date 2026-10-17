---
title: "Rectangle"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Beskriver ett rektangulärt område på en sida eller bild, till exempel OCR-textgränser eller en redigeringsruta."
type: docs
weight: 350
url: /sv/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Beskriver ett rektangulärt område på en sida eller bild, till exempel OCR-textgränser eller en redigeringsruta.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Skapar en rektangel från en övre‑vänsterpunkt och regionens storlek. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Skapar en rektangel från hörnkoordinater och dimensioner. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | En rektangel med noll bredd och höjd vid origo. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Höjd på området, i pixlar. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Hämtar ett värde som indikerar om rektangeln är tom. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Övre‑vänstra hörnet på rektangeln. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Bredd och höjd på rektangeln. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Bredd på området, i pixlar. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Horisontell position för det övre‑vänstra hörnet, i pixlar. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Vertikal position för det övre‑vänstra hörnet, i pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Jämför den här rektangeln med ett annat objekt. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Jämför gränser med en annan rektangel. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Returnerar en hashkod härledd från position och storlek. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Returnerar gränserna i ett läsbart format. |

### Se även

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
