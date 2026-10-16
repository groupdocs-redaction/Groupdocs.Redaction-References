---
title: "Rectangle"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Décrit une zone rectangulaire sur une page ou une image, par exemple les limites de texte OCR ou une boîte de rédaction."
type: docs
weight: 350
url: /fr/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Décrit une zone rectangulaire sur une page ou une image, par exemple les limites d'un texte OCR ou une boîte de rédaction.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Crée un rectangle à partir d'un point en haut à gauche et de la taille de la région. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Crée un rectangle à partir des coordonnées des coins et des dimensions. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | Un rectangle de largeur et hauteur nulles à l'origine. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Hauteur de la zone, en pixels. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Obtient une valeur indiquant si le rectangle est vide. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Coin supérieur gauche du rectangle. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Largeur et hauteur du rectangle. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Largeur de la zone, en pixels. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Position horizontale du coin supérieur gauche, en pixels. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Position verticale du coin supérieur gauche, en pixels. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Compare ce rectangle avec un autre objet. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Compare les limites avec un autre rectangle. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Renvoie un code de hachage dérivé de la position et de la taille. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Renvoie les limites sous une forme lisible. |

### Voir aussi

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
