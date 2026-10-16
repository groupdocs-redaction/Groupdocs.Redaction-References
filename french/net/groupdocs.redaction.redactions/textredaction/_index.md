---
title: "TextRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une classe abstraite de base pour les rédactions de texte de document."
type: docs
weight: 800
url: /fr/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Représente une classe abstraite de base pour les rédactions de texte de document.

```csharp
public abstract class TextRedaction : Redaction
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient l'instance [`ReplacementOptions`](../replacementoptions), spécifiant le type de remplacement de texte. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit l'implémentation [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), requise pour extraire le texte du contenu graphique. |

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
