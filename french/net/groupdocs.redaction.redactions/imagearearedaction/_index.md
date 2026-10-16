---
title: "ImageAreaRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction qui place un rectangle coloré dans la zone donnée d'un document image."
type: docs
weight: 630
url: /fr/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Représente une rédaction qui place un rectangle coloré dans la zone donnée d'un document image.

```csharp
public class ImageAreaRedaction : Redaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Initialise une nouvelle instance de la classe ImageAreaRedaction pour censurer une zone de taille spécifique. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Obtient les options [`RegionReplacementOptions`](../regionreplacementoptions) avec les paramètres de couleur et de zone. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Obtient la position supérieure gauche de la zone à supprimer |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Exemples

L'exemple suivant montre le remplacement d'une zone de l'image par un rectangle de couleur unie.

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

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
