---
title: "DeleteAnnotationRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de texte qui supprime les annotations si le texte correspond à l'expression régulière donnée, supprime éventuellement toutes les annotations."
type: docs
weight: 580
url: /fr/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Représente une rédaction de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, avec des paramètres pour supprimer toutes les annotations (correspondant à tout). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l'expression donnée. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l'expression donnée. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Obtient l'expression régulière à correspondre. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exemples

L'exemple suivant montre comment supprimer toutes les annotations contenant les mots \"use\", \"show\" ou \"describe\" du document (et laisser les autres).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
