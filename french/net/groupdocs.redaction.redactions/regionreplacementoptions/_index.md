---
title: "RegionReplacementOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente les paramètres de couleur et de zone pour le remplacement de région d'image. Voir ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /fr/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Représente les paramètres de couleur et de zone pour le remplacement de région d'image. Voir [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Initialise une nouvelle instance de la classe RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Initialise une nouvelle instance de la classe RegionReplacementOptions dont la taille correspond au texte donné. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Obtient ou définit la couleur pour remplir la zone censurée. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Obtient ou définit le rectangle avec largeur et hauteur. |

### Remarques

**Learn more**

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

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
