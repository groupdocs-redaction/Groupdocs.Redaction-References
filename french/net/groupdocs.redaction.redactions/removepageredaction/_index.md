---
title: "RemovePageRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction qui supprime une page, une diapositive, une feuille de calcul, etc. d'un document."
type: docs
weight: 770
url: /fr/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document.

```csharp
public class RemovePageRedaction : Redaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Initialise une nouvelle instance de la classe RemovePageRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Obtient le nombre de pages à supprimer. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Obtient l'index de position de départ (à partir de 0). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Obtient la position de référence de recherche, le début ou la fin d'un document. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Exemples

L'exemple suivant montre comment supprimer la dernière page du document.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
