---
title: "GroupDocs.Redaction.Integration"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Integration‑namnrymden tillhandahåller gränssnitt och klasser som används för att integrera dokument i olika format med GroupDocs.Redaction."
type: docs
weight: 40
url: /sv/net/groupdocs.redaction.integration/
---
Integration‑namnrymden tillhandahåller gränssnitt och klasser som används för att integrera dokument i olika format med GroupDocs.Redaction.

## Klasser

| Klass | Beskrivning |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Representerar ett specifikt format för ett dokument. Implementera denna klass för att lägga till egna dokumenttyper. |
| [MetadataCollection](./metadatacollection) | Representerar en ordbok av [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) med dess titel som nyckel. |
| [MetadataItem](./metadataitem) | Representerar ett metadataobjekt, gemensamt för alla stödda format och använt i metadata‑maskeringar. |
## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Definierar metoder som krävs för åtkomst till annotationer, såsom kommentarer. Måste implementeras av en klass som härstammar från [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) för att utföra annotation‑maskeringar. |
| [ICellularFormatInstance](./icellularformatinstance) | Definierar metoder som krävs för åtkomst till kalkylbladsformat, med ett eller flera arbetsblad. |
| [IFixedFormatDocument](./ifixedformatdocument) | Definierar metoder som krävs för åtkomstformat med fast struktur, såsom PDF eller presentationer. |
| [IImageFormatInstance](./iimageformatinstance) | Definierar metoder som krävs för redigering av rasterbildformat. |
| [IMetadataAccess](./imetadataaccess) | Definierar metoder som krävs för åtkomst till metadata för ett dokument, om formatet stödjer det. |
| [IPaginatedDocument](./ipaginateddocument) | Definierar metoder som krävs för att manipulera ett dokuments sidor. Måste implementeras av en klass som är härledd från [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) för att utföra sidredigering. |
| [IPreviewable](./ipreviewable) | Definierar metoder för att skapa en förhandsgranskning av dokumentet. |
| [IRasterizableDocument](./irasterizabledocument) | Definierar metoder som krävs för att spara dokument i någon binär form. Inbyggda typer sparar ett dokument som en PDF med bilder av dess sidor. |
| [ITextualFormatInstance](./itextualformatinstance) | Definierar metoder som krävs för att redigera textdata i vilket dokument som helst som innehåller text. |

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
