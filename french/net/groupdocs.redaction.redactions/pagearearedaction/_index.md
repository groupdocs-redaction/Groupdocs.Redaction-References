---
title: "PageAreaRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction textuelle complexe qui affecte le texte, les images et les annotations dans une zone de la page."
type: docs
weight: 680
url: /fr/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Représente une rédaction textuelle complexe qui affecte le texte, les images et les annotations dans une zone de la page.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | Initialise une nouvelle instance de la classe PageAreaRedaction. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | Initialise une nouvelle instance de la classe PageAreaRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient l'instance [`ReplacementOptions`](../replacementoptions), spécifiant le type de remplacement de texte. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Obtient les options [`RegionReplacementOptions`](../regionreplacementoptions) avec les paramètres de couleur et de zone. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit l'implémentation [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), requise pour extraire le texte du contenu graphique. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Obtient l'expression régulière à correspondre. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Voir aussi

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
