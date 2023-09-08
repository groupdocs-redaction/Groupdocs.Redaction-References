---
title: com.groupdocs.redaction.redactions
second_title: GroupDocs.Redaction for Java API Reference
description: The package provides classes for different types of redactions.
type: docs
weight: 16
url: /java/com.groupdocs.redaction.redactions/
---

The package provides classes for different types of redactions.


## Classes

| Class | Description |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Represents a text redaction that replaces text in a spreadsheet documents (CSV, Excel, etc.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Provides an option to limit the scope of a  CellColumnRedaction  to a worksheet and a column. |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Represents a text redaction that deletes annotations if text is matching given regular expression (optionally deletes all annotations). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Represents a text redaction that replaces exact phrase in the document's text, case insensitive by default. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Represents a redaction that places colored rectangle in given area of an image document. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Represents a list of the most common types of document metadata. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Represents a base abstract class for document metadata redactions. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Represents redaction filter, setting an area within a page of a document to apply redaction. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Represents a complex textual redaction that affects text, images and annotations in an area of the page. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Represents redaction filter, setting page range inside a document to apply redaction. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Represents a single change action info that performed during redaction process. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Represents redaction filter, setting scope inside a document to apply redactions. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Represents a text redaction that searches and replaces text in the document by matching provided regular expression. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Represents color and area parameters for image region replacement. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Represents a redaction that removes a page (slide, worksheet, etc.) from a document. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Represents options for matched text replacement. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Represents a base abstract class for document text redactions. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Represents a textual replacement information. |

## Interfaces

| Interface | Description |
| --- | --- |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Defines methods that are required for receiving information on each redaction change and optionally prevent it. |

## Enumerations

| Enum | Description |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Provides the fields that represent reference points in a document for seeking. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Represents actions that can be taken to perform redaction. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Represents a type of document's data, affected by redaction. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Represents a type of replacement for the matched text. |
