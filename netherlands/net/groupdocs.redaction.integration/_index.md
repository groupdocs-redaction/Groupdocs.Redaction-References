---
title: "GroupDocs.Redaction.Integration"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "De Integration namespace biedt interfaces en klassen die worden gebruikt om documenten van verschillende formaten te integreren met GroupDocs.Redaction."
type: docs
weight: 40
url: /nl/net/groupdocs.redaction.integration/
---
De Integration namespace biedt interfaces en klassen, gebruikt om documenten van verschillende formaten te integreren met GroupDocs.Redaction.

## Klassen

| Klasse | Beschrijving |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Stelt een specifiek documentformaat voor. Implementeer deze klasse om uw eigen documenttypen toe te voegen. |
| [MetadataCollection](./metadatacollection) | Stelt een woordenboek van [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) voor met de titel als sleutel. |
| [MetadataItem](./metadataitem) | Stelt een metadata-item voor, gemeenschappelijk voor alle ondersteunde formaten en gebruikt bij metadata-redigeringen. |
## Interfaces

| Interface | Beschrijving |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Definieert methoden die nodig zijn voor toegang tot annotaties, zoals opmerkingen. Moet worden geïmplementeerd door een van [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) afgeleide klasse om annotatie-redigeringen uit te voeren. |
| [ICellularFormatInstance](./icellularformatinstance) | Definieert methoden die nodig zijn voor toegang tot spreadsheetformaten, met één of meerdere werkbladen. |
| [IFixedFormatDocument](./ifixedformatdocument) | Definieert methoden die vereist zijn voor toegang tot formaten met een vaste structuur, zoals PDF of presentaties. |
| [IImageFormatInstance](./iimageformatinstance) | Definieert methoden die vereist zijn voor redactie van rasterafbeeldingsformaten. |
| [IMetadataAccess](./imetadataaccess) | Definieert methoden die vereist zijn voor toegang tot metadata van een document, indien het formaat dit ondersteunt. |
| [IPaginatedDocument](./ipaginateddocument) | Definieert methoden die vereist zijn om de pagina's van een document te manipuleren. Moet worden geïmplementeerd door een van [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance)-afgeleide klasse om paginaredacties uit te voeren. |
| [IPreviewable](./ipreviewable) | Definieert methoden om een voorbeeld van het document te maken. |
| [IRasterizableDocument](./irasterizabledocument) | Definieert methoden die vereist zijn voor het opslaan van een document in elke binaire vorm. Ingebouwde types slaan een document op als een PDF met afbeeldingen van de pagina's. |
| [ITextualFormatInstance](./itextualformatinstance) | Definieert methoden die vereist zijn voor het redigeren van tekstuele gegevens in elk document dat tekst bevat. |

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
