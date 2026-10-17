---
title: "groupdocs.redaction.integration"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Types sous groupdocs.redaction.integration."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/
is_root: false
weight: 30
---


Types sous `groupdocs.redaction.integration`.

### Classes
| Classe | Description |
| :- | :- |
| [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) | Représente un format spécifique d'un document et peut être implémenté pour ajouter des types de documents personnalisés. |
| [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/) | Définit les méthodes requises pour accéder aux annotations, telles que les commentaires, et doit être implémentée par une classe dérivée de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) pour effectuer les redactions d'annotation. |
| [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/) | Définit les méthodes requises pour accéder aux formats de feuilles de calcul contenant une ou plusieurs feuilles de calcul. |
| [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/) | Définit les méthodes requises pour accéder aux formats à structure fixe, tels que PDF ou les présentations. |
| [`IImageFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/iimageformatinstance/) | Définit les méthodes requises pour les redactions de formats d'images raster. |
| [`IMetadataAccess`](/redaction/python-net/groupdocs.redaction.integration/imetadataaccess/) | Définit les méthodes requises pour accéder aux métadonnées d'un document, si le format les prend en charge. |
| [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/) | Définit les méthodes requises pour manipuler les pages d'un document. Doit être implémentée par une classe dérivée de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) pour effectuer les redactions de pages. |
| [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/) | Définit les méthodes pour créer un aperçu du document. |
| [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/) | Définit les méthodes requises pour enregistrer un document sous n'importe quelle forme binaire. Les types intégrés enregistrent un document en PDF avec les images de ses pages. |
| [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/) | Représente une interface qui définit les méthodes requises pour redacter les données textuelles dans tout document contenant du texte. |
| [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/) | Représente un dictionnaire de [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) avec son titre comme clé. |
| [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) | Représente un élément de métadonnées, commun à tous les formats pris en charge et utilisé dans les censures de métadonnées. |
