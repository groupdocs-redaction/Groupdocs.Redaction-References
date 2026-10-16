---
title: "ExactPhraseRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut."
type: docs
weight: 600
url: /fr/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Représente une rédaction de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Initialise une nouvelle instance de la classe ExactPhraseRedaction en mode insensible à la casse. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Initialise une nouvelle instance de la classe ExactPhraseRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient l'instance [`ReplacementOptions`](../replacementoptions), spécifiant le type de remplacement de texte. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Obtient une valeur indiquant si la recherche est sensible à la casse ou non. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Obtient ou définit une valeur indiquant si ce texte est de droite à gauche ou non, false par défaut. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit l'implémentation [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), requise pour extraire le texte du contenu graphique. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Obtient la chaîne à rechercher et à remplacer |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Exemples

L'exemple suivant montre l'exécution d'une recherche et d'un remplacement de phrase sensible à la casse.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Par défaut, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

L'exemple suivant montre le remplacement d'une phrase (insensible à la casse) par un rectangle rouge uni.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Par défaut, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Voir aussi

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
