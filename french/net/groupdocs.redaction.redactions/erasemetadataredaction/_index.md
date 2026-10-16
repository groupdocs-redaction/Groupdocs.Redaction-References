---
title: "EraseMetadataRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des MetadataFilters spécifiques du document."
type: docs
weight: 590
url: /fr/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Représente une rédaction de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des MetadataFilters spécifiques du document.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Initialise une nouvelle instance de la classe EraseMetadataRedaction, en supprimant toutes les métadonnées. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Initialise une nouvelle instance de la classe EraseMetadataRedaction, en supprimant les métadonnées, correspondant à une combinaison spécifique de [`MetadataFilters`](../metadatafilters). |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Obtient ou définit le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Exemples

L'exemple suivant montre comment supprimer (mettre à des valeurs vides) toutes les métadonnées ou des métadonnées spécifiques.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Effacer Auteur, Responsable et Société
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Effacer toutes les métadonnées
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Voir aussi

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
