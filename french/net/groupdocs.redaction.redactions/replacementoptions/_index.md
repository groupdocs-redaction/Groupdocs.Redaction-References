---
title: "ReplacementOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente les options pour le remplacement du texte correspondant."
type: docs
weight: 780
url: /fr/net/groupdocs.redaction.redactions/replacementoptions/
---
## ReplacementOptions class

Représente les options pour le remplacement du texte correspondant.

```csharp
public class ReplacementOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ReplacementOptions](replacementoptions#constructor)(Color) | Initialise une nouvelle instance de la classe ReplacementOptions avec un rectangle coloré comme option. |
| [ReplacementOptions](replacementoptions#constructor_1)(string) | Initialise une nouvelle instance de la classe ReplacementOptions avec du texte de remplacement comme option. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/replacementoptions/actiontype) { get; } | Obtient l'action de remplacement : dessiner une boîte ou remplacer le texte. |
| [BoxColor](../../groupdocs.redaction.redactions/replacementoptions/boxcolor) { get; set; } | Obtient ou définit la couleur pour l'option DrawBox (ignorée sinon). |
| [CustomRedaction](../../groupdocs.redaction.redactions/replacementoptions/customredaction) { get; set; } | Obtient ou définit un gestionnaire de rédaction personnalisé [`ICustomRedactionHandler`](../icustomredactionhandler) qui permet aux utilisateurs de définir leur propre logique de rédaction. |
| [Filters](../../groupdocs.redaction.redactions/replacementoptions/filters) { get; set; } | Obtient ou définit un tableau de filtres à appliquer avec cette rédaction. |
| [Replacement](../../groupdocs.redaction.redactions/replacementoptions/replacement) { get; set; } | Obtient ou définit la valeur de remplacement textuel. |

### Remarques

**Learn more**

* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

### Voir aussi

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
