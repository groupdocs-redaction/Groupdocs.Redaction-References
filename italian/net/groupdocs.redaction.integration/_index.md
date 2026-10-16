---
title: "GroupDocs.Redaction.Integration"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Lo spazio dei nomi Integration fornisce interfacce e classi utilizzate per integrare documenti di diversi formati con GroupDocs.Redaction."
type: docs
weight: 40
url: /it/net/groupdocs.redaction.integration/
---
Lo spazio dei nomi Integration fornisce interfacce e classi, utilizzate per integrare documenti di diversi formati con GroupDocs.Redaction.

## Classi

| Classe | Descrizione |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Rappresenta un formato specifico di un documento. Implementa questa classe per aggiungere i tuoi tipi di documento. |
| [MetadataCollection](./metadatacollection) | Rappresenta un dizionario di [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) con il suo titolo come chiave. |
| [MetadataItem](./metadataitem) | Rappresenta un elemento di metadati, comune a tutti i formati supportati e utilizzato nelle redazioni di metadati. |
## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Definisce i metodi necessari per accedere alle annotazioni, come i commenti. Deve essere implementato dalla classe derivata da [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) per eseguire le redazioni delle annotazioni. |
| [ICellularFormatInstance](./icellularformatinstance) | Definisce i metodi necessari per accedere ai formati di foglio di calcolo, che contengono uno o più fogli di lavoro. |
| [IFixedFormatDocument](./ifixedformatdocument) | Definisce i metodi necessari per i formati di accesso a strutture fisse, come PDF o presentazioni. |
| [IImageFormatInstance](./iimageformatinstance) | Definisce i metodi necessari per le redazioni di formati immagine raster. |
| [IMetadataAccess](./imetadataaccess) | Definisce i metodi necessari per l'accesso ai metadati di un documento, se il formato lo supporta. |
| [IPaginatedDocument](./ipaginateddocument) | Definisce i metodi necessari per manipolare le pagine di un documento. Deve essere implementato dalla classe derivata da [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) per eseguire le redazioni delle pagine. |
| [IPreviewable](./ipreviewable) | Definisce i metodi per creare l'anteprima del documento. |
| [IRasterizableDocument](./irasterizabledocument) | Definisce i metodi necessari per salvare il documento in qualsiasi forma binaria. I tipi integrati salvano un documento come PDF con le immagini delle sue pagine. |
| [ITextualFormatInstance](./itextualformatinstance) | Definisce i metodi necessari per redigere dati testuali in qualsiasi documento, contenente testo. |

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
