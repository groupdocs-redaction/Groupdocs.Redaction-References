---
title: ImageAreaRedaction
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une rédaction qui place un rectangle coloré dans une zone donnée dun document image.
type: docs
weight: 500
url: /fr/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image.

```csharp
public class ImageAreaRedaction : Redaction
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Initialise une nouvelle instance de la classe ImageAreaRedaction pour masquer une taille de zone spécifique. |

## Propriétés

| Nom | La description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Renvoie une chaîne décrivant la rédaction et ses paramètres. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Obtient le[`RegionReplacementOptions`](../regionreplacementoptions)options avec paramètres de couleur et de zone. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Obtient la position en haut à gauche de la zone à supprimer |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Applique la rédaction à une instance de format donnée. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'application des caviardages : [Les bases de la rédaction](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Plus de détails sur les suppressions d'images : [Caviardages d'images](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Exemples

L'exemple suivant illustre le remplacement d'une zone de l'image par un rectangle de couleur unie.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       System.Drawing.Point samplePoint = new System.Drawing.Point(516, 311);
       System.Drawing.Size sampleSize = new System.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(System.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Voir également

* class [Redaction](../../groupdocs.redaction/redaction)
* espace de noms [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->