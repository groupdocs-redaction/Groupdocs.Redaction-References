---
title: "com.groupdocs.redaction.integration"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Le package fournit des interfaces et des classes utilisées pour intégrer des documents de différents formats avec GroupDocs.Redactions."
type: docs
weight: 13
url: /fr/java/com.groupdocs.redaction.integration/
---

Le package fournit des interfaces et des classes, utilisées pour intégrer des documents de différents formats avec GroupDocs.Redactions.



## Classes

| Classe | Description |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Représente un format spécifique d'un document. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Représente un dictionnaire de MetadataItem avec son titre comme clé. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Représente un élément de métadonnées, commun à tous les formats pris en charge et utilisé dans les suppressions de métadonnées. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Représente du texte, extrait d'une image à la suite de son processus de reconnaissance. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Fournit une façade pour toutes les opérations de suppression d'images raster. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Représente une partie du texte reconnu (mot, symbole, etc.), extrait par le moteur OCR. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Représente une ligne de texte, extraite par le moteur OCR d'une image. |

## Interfaces

| Interface | Description |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Définit les méthodes nécessaires pour accéder aux annotations, telles que les commentaires. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Définit les méthodes nécessaires pour accéder aux formats de feuilles de calcul, comportant une ou plusieurs feuilles de calcul. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Définit les méthodes nécessaires pour accéder aux formats à structure fixe, tels que PDF ou les présentations. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Définit les méthodes nécessaires pour les suppressions de formats d'images raster. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Définit les méthodes nécessaires pour accéder aux métadonnées d'un document, si le format le prend en charge. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Définit les méthodes nécessaires pour supprimer plusieurs zones d'image en même temps avec la même couleur. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Définit les méthodes nécessaires pour appliquer des suppressions textuelles aux documents image et aux images intégrées. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Définit les méthodes nécessaires pour manipuler les pages d'un document. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Définit les méthodes pour créer un aperçu du document. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Définit les méthodes nécessaires pour enregistrer le document sous n'importe quelle forme binaire. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Définit les méthodes nécessaires pour supprimer les données textuelles dans tout document contenant du texte. |
