---
title: "MetadataSearchRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en metadata‑radering som söker och raderar metadata med hjälp av reguljära uttryck, matchar nycklar och/eller värden."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Representerar en metadata‑radering som söker och raderar metadata med hjälp av reguljära uttryck, matchar nycklar och/eller värden.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Initierar en ny instans av MetadataSearchRedaction-klassen med värde för att matcha redigerade objekt. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Initierar en ny instans av MetadataSearchRedaction med objektnamn och värde för att matcha redigerade objekt. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Initierar en ny instans av MetadataSearchRedaction-klassen med värde för att matcha redigerade objekt. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Initierar en ny instans av MetadataSearchRedaction med objektnamn och värde för att matcha redigerade objekt. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Tillämpar maskeringen på en given formatinstans. (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Beskrivningen av redigeringen, som innehåller dess namn och parametrar. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Reguljärt uttryck för att matcha namnet (nyckeln) på ett metadataobjekt. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Det textuella ersättningsvärdet. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Reguljärt uttryck för att matcha värdetexten för ett metadataobjekt. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Filtret som används för att välja all eller specifik metadata, såsom Author eller Company. (ärvd från [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Maskera alla metadata‑värden som matchar mönstret
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Uppgiftsguider som använder `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
