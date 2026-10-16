---
title: "MetadataSearchRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de métadonnées qui recherche et censure les métadonnées en utilisant des expressions régulières correspondant aux clés et/ou aux valeurs."
type: docs
weight: 660
url: /fr/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Représente une rédaction de métadonnées qui recherche et rédige les métadonnées à l'aide d'expressions régulières, en faisant correspondre les clés et/ou les valeurs.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour faire correspondre les éléments censurés. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour faire correspondre les éléments censurés. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant le nom de l'élément et la valeur pour faire correspondre les éléments censurés. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant le nom de l'élément et la valeur pour faire correspondre les éléments censurés. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Obtient ou définit le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Obtient l'expression régulière pour faire correspondre le nom (clé) d'un élément de métadonnées. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Obtient la valeur de remplacement textuelle. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Obtient l'expression régulière pour faire correspondre le texte de la valeur d'un élément de métadonnées. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Exemples

L'exemple suivant montre comment rechercher et censurer un certain texte dans des métadonnées spécifiques.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Si non défini, s'applique à tous les éléments de métadonnées
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Voir aussi

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
