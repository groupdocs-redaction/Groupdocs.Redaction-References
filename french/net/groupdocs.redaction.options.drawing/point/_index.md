---
title: "Point"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Identifie un décalage en pixels sur une page ou une image, généralement le coin supérieur gauche d’une zone de rédaction."
type: docs
weight: 340
url: /fr/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Identifie un décalage en pixels sur une page ou une image, généralement le coin supérieur gauche d'une zone de rédaction.

```csharp
public struct Point : IEquatable<Point>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Point](point)(int, int) | Crée un point pour l’origine d’une région de rédaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | Un point à l’origine (0, 0). |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Décalage horizontal depuis le bord gauche, en pixels. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Décalage vertical depuis le bord supérieur, en pixels. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Compare ce point avec un autre objet. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Compare les coordonnées avec un autre point. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Renvoie un code de hachage dérivé des coordonnées. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Renvoie les coordonnées sous une forme lisible. |

### Voir aussi

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
