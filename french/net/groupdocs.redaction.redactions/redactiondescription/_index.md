---
title: "RedactionDescription"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une information sur une action de modification unique effectuée pendant le processus de rédaction."
type: docs
weight: 720
url: /fr/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Représente une information sur une action de modification unique effectuée pendant le processus de rédaction.

```csharp
public class RedactionDescription
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement de zone d'image. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Obtient l'opération de censure : remplacement, nettoyage ou suppression. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Obtient ou définit des informations détaillées facultatives pour l'élément censuré. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Obtient les informations de remplacement pour les censures de zones d'image, renvoie null pour les censures textuelles. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Obtient le texte correspondant, si une expression est fournie. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Obtient le type de données du document - texte, métadonnées ou annotations. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Obtient les informations de remplacement, peut être null. |

### Remarques

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Voir aussi

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
