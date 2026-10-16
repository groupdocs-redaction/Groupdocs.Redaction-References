---
title: "GroupDocs.Redaction.Integration"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "L’espace de noms Integration fournit des interfaces et des classes utilisées pour intégrer des documents de différents formats avec GroupDocs.Redaction."
type: docs
weight: 40
url: /fr/net/groupdocs.redaction.integration/
---
L’espace de noms Integration fournit des interfaces et des classes, utilisées pour intégrer des documents de différents formats avec GroupDocs.Redaction.

## Classes

| Classe | Description |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Représente un format spécifique d’un document. Implémentez cette classe pour ajouter vos propres types de documents. |
| [MetadataCollection](./metadatacollection) | Représente un dictionnaire de [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) avec son titre comme clé. |
| [MetadataItem](./metadataitem) | Représente un élément de métadonnées, commun à tous les formats pris en charge et utilisé dans les masquages de métadonnées. |
## Interfaces

| Interface | Description |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Définit les méthodes requises pour accéder aux annotations, telles que les commentaires. Doit être implémentée par la classe dérivée de [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) pour effectuer les masquages d’annotations. |
| [ICellularFormatInstance](./icellularformatinstance) | Définit les méthodes requises pour accéder aux formats de feuilles de calcul, possédant une ou plusieurs feuilles de calcul. |
| [IFixedFormatDocument](./ifixedformatdocument) | Définit les méthodes nécessaires pour accéder aux formats à structure fixe, tels que PDF ou les présentations. |
| [IImageFormatInstance](./iimageformatinstance) | Définit les méthodes requises pour les rédactions de formats d'images raster. |
| [IMetadataAccess](./imetadataaccess) | Définit les méthodes nécessaires pour accéder aux métadonnées d'un document, si le format le prend en charge. |
| [IPaginatedDocument](./ipaginateddocument) | Définit les méthodes nécessaires pour manipuler les pages d'un document. Doit être implémentée par la classe dérivée de [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) pour effectuer les rédactions de pages. |
| [IPreviewable](./ipreviewable) | Définit les méthodes pour créer un aperçu du document. |
| [IRasterizableDocument](./irasterizabledocument) | Définit les méthodes requises pour enregistrer un document sous n'importe quelle forme binaire. Les types intégrés enregistrent un document en PDF avec les images de ses pages. |
| [ITextualFormatInstance](./itextualformatinstance) | Définit les méthodes nécessaires pour la rédaction de données textuelles dans tout document contenant du texte. |

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
