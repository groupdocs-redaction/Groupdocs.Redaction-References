---
title: MetadataRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a base abstract class for document metadata redactions."
type: docs
url: /python-net/groupdocs.redaction.redactions/metadataredaction/
is_root: false
weight: 130
---


## MetadataRedaction class

Represents a base abstract class for document metadata redactions.

Base functionality for all redactions, derived from [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) base class is metadata filtering and it is mandatory for metadata redactions. It uses the flagged enumeration `MetadataFilters`, containing items for the most frequent metadata entries. You can set the filter to `All`, or any combination of metadata.

- More details about document metadata redactions: https://docs.groupdocs.com/redaction/python-net/metadata-redactions/

The MetadataRedaction type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | The filter used to select all or specific metadata, such as Author or Company. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | The description of the redaction, describing the redaction and its parameters. (inherited from [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Guides
Task guides that use `MetadataRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
