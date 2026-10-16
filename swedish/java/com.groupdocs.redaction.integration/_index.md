---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Paketet tillhandahåller gränssnitt och klasser som används för att integrera dokument i olika format med GroupDocs.Redactions."
type: docs
weight: 13
url: /sv/java/com.groupdocs.redaction.integration/
---

Paketet tillhandahåller gränssnitt och klasser som används för att integrera dokument av olika format med GroupDocs.Redactions.



## Klasser

| Klass | Beskrivning |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Representerar ett specifikt format för ett dokument. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Representerar en ordbok av MetadataItem med dess titel som nyckel. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Representerar ett metadataobjekt, gemensamt för alla stödda format och som används i metadata‑redigeringar. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Representerar text som extraheras från en bild som resultat av dess igenkänningsprocess. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Tillhandahåller en fasad till alla rasterbildsredigeringsoperationer. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Representerar en del av igenkänd text (ord, symbol osv), extraherad av OCR‑motorn. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Representerar en textrad, extraherad av OCR‑motorn från en bild. |

## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Definierar metoder som krävs för åtkomst till annotationer, såsom kommentarer. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Definierar metoder som krävs för åtkomst till kalkylbladsformat, med ett eller flera kalkylblad. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Definierar metoder som krävs för åtkomst till format med fast struktur, såsom PDF eller presentationer. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Definierar metoder som krävs för redigering av rasterbildsformat. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Definierar metoder som krävs för åtkomst till metadata för ett dokument, om formatet stöder det. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Definierar metoder som krävs för att redigera flera bildområden samtidigt med samma färg. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Definierar metoder som krävs för att tillämpa textredigeringar på bilddokument och inbäddade bilder. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Definierar metoder som krävs för att manipulera ett dokuments sidor. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Definierar metoder för att skapa en förhandsgranskning av dokumentet. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Definierar metoder som krävs för att spara dokumentet i någon binär form. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Definierar metoder som krävs för att redigera textdata i vilket dokument som helst, som innehåller text. |
