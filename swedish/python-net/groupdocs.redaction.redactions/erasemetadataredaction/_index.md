---
title: "EraseMetadataRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en metadata-maskering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Representerar en metadata-maskering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

EraseMetadataRedaction-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Initierar en ny instans av EraseMetadataRedaction-klass, som raderar all metadata. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Initierar en ny instans av EraseMetadataRedaction, raderar metadata som matchar de angivna `MetadataFilters`. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Tillämpar maskeringen på en given formatinstans. (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Beskrivningen av maskeringen och dess parametrar. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Filtret som används för att välja all eller specifik metadata, såsom Author eller Company. (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Radera all metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Radera endast författarfältet
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Uppgiftsguider som använder `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
