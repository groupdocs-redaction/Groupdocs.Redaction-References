---
title: "AnnotationRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction qui remplace le texte, les commentaires, etc. des annotations correspondant à une expression régulière donnée."
type: docs
weight: 530
url: /fr/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Représente une rédaction qui remplace le texte d'annotation (commentaires, etc.) correspondant à une expression régulière donnée.

```csharp
public class AnnotationRedaction : Redaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Initialise une nouvelle instance de la classe AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Initialise une nouvelle instance de la classe AnnotationRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Obtient l'expression régulière à correspondre. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Obtient un remplacement textuel pour le texte correspondant. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exemples

L'exemple suivant montre comment remplacer le nom "John" par "[redacted]" dans toutes les annotations.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
