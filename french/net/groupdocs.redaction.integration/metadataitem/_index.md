---
title: "MetadataItem"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente un élément de métadonnées commun à tous les formats pris en charge et utilisé dans les rédactions de métadonnées."
type: docs
weight: 220
url: /fr/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Représente un élément de métadonnées, commun à tous les formats pris en charge et utilisé dans les masquages de métadonnées.

```csharp
public class MetadataItem : ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MetadataItem](metadataitem)() | Initialise une nouvelle instance. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Obtient la représentation sous forme de chaîne de la valeur de l'élément de métadonnées. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Obtient ou définit une catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource incorporée. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Obtient une clé de dictionnaire pour [`MetadataCollection`](../metadatacollection), en utilisant son OriginalName et d'autres données. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Obtient ou définit une valeur de [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters), assignée à cet élément de métadonnées et utilisée dans le filtrage des éléments. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Obtient ou définit une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Obtient ou définit le nom original de l'élément de métadonnées, tel qu'il apparaît dans le document. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Obtient ou définit la valeur de l'élément de métadonnées. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Crée un clone profond de l'instance actuelle. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Renvoie des informations sur les propriétés sérialisables. |

### Voir aussi

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
