---
title: groupdocs.redaction.redactions
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Types under groupdocs.redaction.redactions."
type: docs
url: /python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


Types under `groupdocs.redaction.redactions`.

### Classes
| Class | Description |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | Represents a redaction that replaces annotation text (comments, etc.) matching a given regular expression. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | Represents a text redaction that replaces text in a spreadsheet document (CSV, Excel, etc.). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | Provides an option to limit the scope of a [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) to a worksheet and a column. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | Provides context for custom redaction processing. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | Represents the result of a custom redaction operation. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | Represents a text redaction that deletes annotations if text matches a given regular expression (optionally deletes all annotations). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | Represents a metadata redaction that erases all metadata or metadata matching specific MetadataFilters from the document. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | Represents a text redaction that replaces an exact phrase in the document's text, case insensitive by default. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | Provides an interface for implementing custom redaction logic. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | Defines methods required for receiving information on each redaction change and optionally preventing it. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | Represents a redaction that places a colored rectangle in a given area of an image document. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | Represents a base abstract class for document metadata redactions. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | Represents redaction filter, setting an area within a page of a document to apply redaction. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | Represents a complex textual redaction that affects text, images and annotations in an area of the page. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | Represents redaction filter, setting page range inside a document to apply redaction. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | Represents a single change action info that performed during redaction process. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Represents a text redaction that searches and replaces text in the document by matching provided regular expression. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | Represents color and area parameters for image region replacement. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | Represents a redaction that removes a page (slide, worksheet, etc.) from a document. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | Represents options for matched text replacement. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | Represents a base abstract class for document text redactions. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | Represents a textual replacement information. |

### Enumerations
| Enum | Description |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | Represents redaction filter, setting scope inside a document to apply redactions. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
