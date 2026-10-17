---
title: "groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Typer under groupdocs.redaction.integration."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/
is_root: false
weight: 30
---


Typer under `groupdocs.redaction.integration`.

### Klasser
| Klass | Beskrivning |
| :- | :- |
| [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) | Representerar ett specifikt format för ett dokument och kan implementeras för att lägga till anpassade dokumenttyper. |
| [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/) | Definierar metoder som krävs för att komma åt annotationer, såsom kommentarer, och måste implementeras av en [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-avledd klass för att utföra annotationredigeringar. |
| [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/) | Definierar metoder som krävs för att komma åt kalkylbladsformat som innehåller ett eller flera arbetsblad. |
| [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/) | Definierar metoder som krävs för åtkomst till format med fast struktur, såsom PDF eller presentationer. |
| [`IImageFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/iimageformatinstance/) | Definierar metoder som krävs för rasterbildformatredigeringar. |
| [`IMetadataAccess`](/redaction/python-net/groupdocs.redaction.integration/imetadataaccess/) | Definierar metoder som krävs för åtkomst till metadata för ett dokument, om formatet stödjer det. |
| [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/) | Definierar metoder som krävs för att manipulera ett dokuments sidor. Måste implementeras av en [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-avledd klass för att utföra sidredigeringar. |
| [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/) | Definierar metoder för att skapa en förhandsgranskning av dokumentet. |
| [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/) | Definierar metoder som krävs för att spara ett dokument i någon binär form. Inbyggda typer sparar ett dokument som en PDF med bilder av dess sidor. |
| [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/) | Representerar ett gränssnitt som definierar metoder som krävs för att redigera textdata i vilket dokument som helst som innehåller text. |
| [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/) | Representerar en ordbok av [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) med dess titel som nyckel. |
| [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) | Representerar ett metadata-objekt, gemensamt för alla stödda format och som används i metadata-redigeringar. |
