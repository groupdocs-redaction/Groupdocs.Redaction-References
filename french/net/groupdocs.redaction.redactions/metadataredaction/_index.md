---
title: "MetadataRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une classe abstraite de base pour les rédactions de métadonnées de document."
type: docs
weight: 650
url: /fr/net/groupdocs.redaction.redactions/metadataredaction/
---
## MetadataRedaction class

Représente une classe abstraite de base pour les rédactions de métadonnées de document.

```csharp
public abstract class MetadataRedaction : Redaction
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Obtient ou définit le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Voir aussi

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
