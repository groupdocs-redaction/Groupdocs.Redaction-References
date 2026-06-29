---
title: groupdocs.redaction.integration
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Types under groupdocs.redaction.integration."
type: docs
url: /python-net/groupdocs.redaction.integration/
is_root: false
weight: 30
---


Types under `groupdocs.redaction.integration`.

### Classes
| Class | Description |
| :- | :- |
| [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) | Represents a specific format of a document and can be implemented to add custom document types. |
| [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/) | Defines methods required for accessing annotations, such as comments, and must be implemented by a [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-derived class to perform annotation redactions. |
| [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/) | Defines methods required for accessing spreadsheet formats that contain one or many worksheets. |
| [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/) | Defines methods that are required for access formats of fixed structure, such as PDF or presentations. |
| [`IImageFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/iimageformatinstance/) | Defines methods required for raster image format redactions. |
| [`IMetadataAccess`](/redaction/python-net/groupdocs.redaction.integration/imetadataaccess/) | Defines methods that are required for access to metadata of a document, if the format supports it. |
| [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/) | Defines methods that are required to manipulate a document's pages. Needs to be implemented by [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-derived class to perform page redactions. |
| [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/) | Defines methods to create a preview of the document. |
| [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/) | Defines methods required for saving a document in any binary form. Built-in types save a document as a PDF with images of its pages. |
| [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/) | Represents an interface that defines methods required for redacting textual data in any document containing text. |
| [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/) | Represents a dictionary of [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) with its title as a key. |
| [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) | Represents an item of metadata, common for all supported formats and used in metadata redactions. |
