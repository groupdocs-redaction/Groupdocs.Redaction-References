---
title: "RegexRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie."
type: docs
weight: 750
url: /fr/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie.

```csharp
public class RegexRedaction : TextRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Initialise une nouvelle instance de la classe RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Initialise une nouvelle instance de la classe RegexRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient l'instance [`ReplacementOptions`](../replacementoptions), spécifiant le type de remplacement de texte. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit l'implémentation [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), requise pour extraire le texte du contenu graphique. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Obtient l'expression régulière à correspondre. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Exemples

L'exemple suivant montre le remplacement de texte à l'aide de l'expression régulière.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // remplacer par du texte
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // remplacer par un rectangle bleu plein
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Voir aussi

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
