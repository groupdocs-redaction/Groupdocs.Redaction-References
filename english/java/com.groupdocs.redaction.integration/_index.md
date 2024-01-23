---
title: com.groupdocs.redaction.integration
second_title: GroupDocs.Redaction for Java API Reference
description: The package provides interfaces and classes used to integrate documents of different formats with GroupDocs.Redactions.
type: docs
weight: 13
url: /java/com.groupdocs.redaction.integration/
---

The package provides interfaces and classes, used to integrate documents of different formats with GroupDocs.Redactions.


## Classes

| Class | Description |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Represents a specific format of a document. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Represents a dictionary of  MetadataItem  with its title as a key. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Represents an item of metadata, common for all supported formats and used in metadata redactions. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Represents text, extracted from an image as a result of its recognition process. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Provides facade to all raster image redaction operations. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Represents a part of recognized text (word, symbol, etc), extracted by OCR engine. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Represents a line of text, extracted by OCR engine from an image. |

## Interfaces

| Interface | Description |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Defines methods that are required for access to annotations, such as comments. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Defines methods that are required for access to spreadsheet formats, having one or many worksheets. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Defines methods that are required for access formats of fixed structure, such as PDF or presentations. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Defines methods that are required for raster image format redactions. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Defines methods that are required for access to metadata of a document, if format supports it. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Defines methods that are required to redact multiple image areas at once with the same color. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Defines methods that are required to apply textual redactions to image documents and embedded images. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Defines methods that are required to manipulate a document's pages. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Defines methods to create preview of the document. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Defines methods that are required for saving document in any binary form. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Defines methods that are required for redacting textual data in any document, containing text. |
