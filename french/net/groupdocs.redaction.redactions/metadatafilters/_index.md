---
title: "MetadataFilters"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une liste des types de métadonnées de document les plus courants."
type: docs
weight: 640
url: /fr/net/groupdocs.redaction.redactions/metadatafilters/
---
## MetadataFilters enumeration

Représente une liste des types de métadonnées de document les plus courants.

```csharp
[Flags]
public enum MetadataFilters
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Paramètre de filtre vide, ne correspond à aucun élément de métadonnées. |
| Author | `1` | Auteur du document. |
| Category | `2` | Catégorie du document. |
| Comments | `4` | Commentaire du document. |
| Company | `8` | Entreprise de l'auteur. |
| ContentStatus | `10` | État du contenu. |
| CreatedTime | `20` | Date de création. |
| HyperlinkBase | `40` | Base du lien hypertexte. |
| LastPrinted | `80` | Date et heure de la dernière impression. |
| LastSavedBy | `100` | Dernière sauvegarde par l'utilisateur. |
| LastSavedTime | `400` | Date et heure de la dernière sauvegarde. |
| NameOfApplication | `800` | Nom de l'application où le document a été créé. |
| Manager | `1000` | Nom du responsable de l'auteur. |
| RevisionNumber | `2000` | Numéro de révision. |
| Subject | `4000` | Sujet du document. |
| Template | `8000` | Nom du modèle de document. |
| Title | `10000` | Titre du document. |
| TotalEditingTime | `20000` | Temps total d'édition. |
| Version | `40000` | Version du document. |
| Description | `80000` | Description du document. |
| Keywords | `100000` | Mots-clés du document. |
| ContentType | `200000` | Type de contenu. |
| All | `7FFFFFFF` | Tous les types d'éléments de métadonnées. |

### Remarques

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Voir aussi

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
