---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Het pakket biedt interfaces en klassen die worden gebruikt om documenten van verschillende formaten te integreren met GroupDocs.Redactions."
type: docs
weight: 13
url: /nl/java/com.groupdocs.redaction.integration/
---

Het pakket biedt interfaces en klassen, gebruikt om documenten van verschillende formaten te integreren met GroupDocs.Redactions.



## Klassen

| Klasse | Beschrijving |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Vertegenwoordigt een specifiek formaat van een document. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Stelt een woordenboek van MetadataItem voor met de titel als sleutel. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Stelt een metadata-item voor, gemeenschappelijk voor alle ondersteunde formaten en gebruikt bij metadata-redacties. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Stelt tekst voor, geëxtraheerd uit een afbeelding als resultaat van het herkenningsproces. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Biedt een façade voor alle rasterafbeelding-redactiebewerkingen. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Stelt een deel van herkende tekst (woord, symbool, enz.) voor, geëxtraheerd door de OCR-engine. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Stelt een regel tekst voor, geëxtraheerd door de OCR-engine uit een afbeelding. |

## Interfaces

| Interface | Beschrijving |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Definieert methoden die nodig zijn voor toegang tot annotaties, zoals opmerkingen. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Definieert methoden die nodig zijn voor toegang tot spreadsheetformaten, met één of meerdere werkbladen. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Definieert methoden die nodig zijn voor toegang tot formaten met een vaste structuur, zoals PDF of presentaties. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Definieert methoden die nodig zijn voor redacties van rasterafbeeldingsformaten. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Definieert methoden die nodig zijn voor toegang tot metadata van een document, indien het formaat dit ondersteunt. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Definieert methoden die nodig zijn om meerdere afbeeldingsgebieden in één keer te redigeren met dezelfde kleur. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Definieert methoden die nodig zijn om tekstuele redacties toe te passen op afbeeldingsdocumenten en ingesloten afbeeldingen. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Definieert methoden die nodig zijn om de pagina's van een document te manipuleren. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Definieert methoden om een voorbeeld van het document te maken. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Definieert methoden die nodig zijn voor het opslaan van een document in elke binaire vorm. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Definieert methoden die nodig zijn voor het redigeren van tekstuele gegevens in elk document dat tekst bevat. |
