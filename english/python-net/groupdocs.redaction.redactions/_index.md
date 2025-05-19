---
title: groupdocs.redaction.redactions
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/
is_root: false
weight: 10
---

The GroupDocs.Redaction namespace provides classes for different types of redactions.

### Classes
| Class | Description |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction) | Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction) | Represents a text redaction that replaces text in a spreadsheet documents (CSV, Excel, etc.). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter) | Provides an option to limit the scope of a [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction) to a worksheet and a column. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext) | Provides context for custom redaction processing. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult) | Represents the result of a custom redaction operation. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction) | Represents a text redaction that deletes annotations if text is matching given regular expression (optionally deletes all annotations). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction) | Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction) | Represents a text redaction that replaces exact phrase in the document's text, case insensitive by default. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler) | Provides an interface for implementing custom redaction logic. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback) | Defines methods that are required for receiving information on each redaction change and optionally prevent it. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction) | Represents a redaction that places colored rectangle in given area of an image document. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction) | Represents a base abstract class for document metadata redactions. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction) | Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter) | Represents redaction filter, setting an area within a page of a document to apply redaction. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction) | Represents a complex textual redaction that affects text, images and annotations in an area of the page. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter) | Represents redaction filter, setting page range inside a document to apply redaction. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription) | Represents a single change action info that performed during redaction process. |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter) | Represents redaction filter, setting scope inside a document to apply redactions. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction) | Represents a text redaction that searches and replaces text in the document by matching provided regular expression. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions) | Represents color and area parameters for image region replacement. See [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction). |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction) | Represents a redaction that removes a page (slide, worksheet, etc.) from a document. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) | Represents options for matched text replacement. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction) | Represents a base abstract class for document text redactions. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement) | Represents a textual replacement information. |


### Enumerations
| Enumeration | Description |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters) | Represents a list of the most common types of document metadata. |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin) | Provides the fields that represent reference points in a document for seeking. |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype) | Represents actions that can be taken to perform redaction. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype) | Represents a type of document's data, affected by redaction. |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype) | Represents a type of replacement for the matched text. |


