---
title: AnnotationRedaction
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une rédaction qui remplace le texte dannotation commentaires etc. correspondant à une expression régulière donnée.
type: docs
weight: 440
url: /fr/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Représente une rédaction qui remplace le texte d'annotation (commentaires, etc.) correspondant à une expression régulière donnée.

```csharp
public class AnnotationRedaction : Redaction
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Initialise une nouvelle instance de la classe AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Initialise une nouvelle instance de la classe AnnotationRedaction. |

## Propriétés

| Nom | La description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Renvoie une chaîne décrivant la rédaction et ses paramètres. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Obtient l'expression régulière correspondant. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Obtient un remplacement textuel pour le texte correspondant. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Applique la rédaction à une instance de format donnée. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'application des caviardages : [Les bases de la rédaction](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Plus de détails sur les suppressions d'annotations de documents : [Caviardages d'annotations](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exemples

L'exemple suivant montre comment remplacer le nom "John" par "[expurgé]" dans toutes les annotations.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Voir également

* class [Redaction](../../groupdocs.redaction/redaction)
* espace de noms [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
