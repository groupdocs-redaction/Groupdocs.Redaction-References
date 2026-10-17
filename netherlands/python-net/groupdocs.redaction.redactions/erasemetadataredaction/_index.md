---
title: "EraseMetadataRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een metadataredactie voor die alle metadata of metadata die overeenkomt met specifieke MetadataFilters uit het document wist."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Stelt een metadataredactie voor die alle metadata of metadata die overeenkomt met specifieke MetadataFilters uit het document wist.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Het type EraseMetadataRedaction exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Initialiseert een nieuwe instantie van de EraseMetadataRedaction klasse, waarbij alle metadata worden gewist. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Initialiseert een nieuw exemplaar van EraseMetadataRedaction, waarbij metadata wordt gewist die overeenkomt met de opgegeven `MetadataFilters`. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Past de redactie toe op een gegeven formaatinstantie. (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | De beschrijving van de redactie en de bijbehorende parameters. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Het filter dat wordt gebruikt om alle of specifieke metadata te selecteren, zoals Auteur of Bedrijf. (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Wis alle metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Wis alleen het auteursveld
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Taakgidsen die `EraseMetadataRedaction` gebruiken:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
