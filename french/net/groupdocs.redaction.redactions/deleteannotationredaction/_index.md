---
title: DeleteAnnotationRedaction
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une rédaction de texte qui supprime les annotations si le texte correspond à lexpression régulière donnée supprime éventuellement toutes les annotations.
type: docs
weight: 460
url: /fr/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Représente une rédaction de texte qui supprime les annotations si le texte correspond à l'expression régulière donnée (supprime éventuellement toutes les annotations).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, avec des paramètres pour supprimer toutes les annotations (correspondant à tout). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, en supprimant les annotations correspondant à l'expression donnée. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, en supprimant les annotations correspondant à l'expression donnée. |

## Propriétés

| Nom | La description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Renvoie une chaîne décrivant la rédaction et ses paramètres. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Obtient l'expression régulière correspondant. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Applique la rédaction à une instance de format donnée. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'application des caviardages : [Les bases de la rédaction](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Plus de détails sur les suppressions d'annotations de documents : [Caviardages d'annotations](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exemples

L'exemple suivant montre comment supprimer toutes les annotations contenant les mots "use", "show" ou "describe" du document (et laisser les autres).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Voir également

* class [Redaction](../../groupdocs.redaction/redaction)
* espace de noms [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->