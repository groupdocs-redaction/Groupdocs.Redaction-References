---
title: "Punt"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Identificeert een pixelverschuiving op een pagina of afbeelding, meestal de linkerbovenhoek van een redactiegebied."
type: docs
weight: 340
url: /nl/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Identificeert een pixelverschuiving op een pagina of afbeelding, meestal de linkerbovenhoek van een redactiegebied.

```csharp
public struct Point : IEquatable<Point>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Point](point)(int, int) | Maakt een punt voor de oorsprong van een redactiegebied. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | Een punt op de oorsprong (0, 0). |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Horizontale verschuiving vanaf de linkerrand, in pixels. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Verticale verschuiving vanaf de bovenzijde, in pixels. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Vergelijkt dit punt met een ander object. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Vergelijkt coördinaten met een ander punt. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Retourneert een hashcode afgeleid van de coördinaten. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Retourneert de coördinaten in een leesbare vorm. |

### Zie ook

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
