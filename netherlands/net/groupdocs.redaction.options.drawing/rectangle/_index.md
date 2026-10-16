---
title: "Rechthoek"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Beschrijft een rechthoekig gebied op een pagina of afbeelding, bijvoorbeeld een OCR-tekstgrens of een redactievak."
type: docs
weight: 350
url: /nl/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Beschrijft een rechthoekig gebied op een pagina of afbeelding, bijvoorbeeld de grenzen van OCR-tekst of een redactie‑vak.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Maakt een rechthoek aan vanuit een linkerbovenpunt en regio-grootte. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Maakt een rechthoek aan vanuit hoekcoördinaten en afmetingen. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | Een rechthoek met nul breedte en hoogte op de oorsprong. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Hoogte van het gebied, in pixels. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Haalt een waarde op die aangeeft of de rechthoek leeg is. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Linkerbovenhoek van de rechthoek. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Breedte en hoogte van de rechthoek. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Breedte van het gebied, in pixels. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Horizontale positie van de linkerbovenhoek, in pixels. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Verticale positie van de linkerbovenhoek, in pixels. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Vergelijkt deze rechthoek met een ander object. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Vergelijkt grenzen met een andere rechthoek. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Retourneert een hashcode afgeleid van positie en grootte. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Retourneert de grenzen in een leesbare vorm. |

### Zie ook

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
