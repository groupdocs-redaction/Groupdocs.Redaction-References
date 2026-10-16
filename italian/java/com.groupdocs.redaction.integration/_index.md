---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Il pacchetto fornisce interfacce e classi utilizzate per integrare documenti di diversi formati con GroupDocs.Redactions."
type: docs
weight: 13
url: /it/java/com.groupdocs.redaction.integration/
---

Il pacchetto fornisce interfacce e classi, utilizzate per integrare documenti di diversi formati con GroupDocs.Redactions.



## Classi

| Classe | Descrizione |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Rappresenta un formato specifico di un documento. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Rappresenta un dizionario di MetadataItem con il suo titolo come chiave. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Rappresenta un elemento di metadati, comune a tutti i formati supportati e utilizzato nelle redazioni dei metadati. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Rappresenta il testo, estratto da un'immagine come risultato del suo processo di riconoscimento. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Fornisce una facciata per tutte le operazioni di redazione di immagini raster. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Rappresenta una parte del testo riconosciuto (parola, simbolo, ecc.), estratta dal motore OCR. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Rappresenta una riga di testo, estratta dal motore OCR da un'immagine. |

## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Definisce i metodi necessari per l'accesso alle annotazioni, come i commenti. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Definisce i metodi necessari per l'accesso ai formati di foglio di calcolo, con uno o più fogli di lavoro. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Definisce i metodi necessari per l'accesso a formati a struttura fissa, come PDF o presentazioni. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Definisce i metodi necessari per le redazioni di formati di immagini raster. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Definisce i metodi necessari per l'accesso ai metadati di un documento, se il formato lo supporta. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Definisce i metodi necessari per redigere più aree immagine contemporaneamente con lo stesso colore. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Definisce i metodi necessari per applicare redazioni testuali a documenti immagine e immagini incorporate. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Definisce i metodi necessari per manipolare le pagine di un documento. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Definisce i metodi per creare un'anteprima del documento. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Definisce i metodi necessari per salvare il documento in qualsiasi forma binaria. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Definisce i metodi necessari per redigere dati testuali in qualsiasi documento, contenente testo. |
