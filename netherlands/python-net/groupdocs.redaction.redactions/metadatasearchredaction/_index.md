---
title: "MetadataSearchRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een metadata‑redactie voor die metadata zoekt en redacteert met behulp van reguliere expressies, waarbij sleutels en/of waarden worden gematcht."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Stelt een metadata‑redactie voor die metadata zoekt en redacteert met behulp van reguliere expressies, waarbij sleutels en/of waarden worden gematcht.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Het type MetadataSearchRedaction biedt de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction klasse, met een waarde om te matchen met geredigeerde items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Initialiseert een nieuw exemplaar van MetadataSearchRedaction, met itemnaam en waarde om te matchen met geredigeerde items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction klasse, met een waarde om te matchen met geredigeerde items. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Initialiseert een nieuw exemplaar van MetadataSearchRedaction met itemnaam en waarde om te matchen met geredigeerde items. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Past de redactie toe op een gegeven formaatinstantie. (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | De beschrijving van de redactie, met de naam en parameters. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | De reguliere expressie om de naam (sleutel) van een metadata-item te matchen. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | De tekstuele vervangingswaarde. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | De reguliere expressie om de waardetekst van een metadata-item te matchen. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Het filter dat wordt gebruikt om alle of specifieke metadata te selecteren, zoals Auteur of Bedrijf. (geërfd van [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Redigeer elke metadata-waarde die overeenkomt met het patroon
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Taakgidsen die `MetadataSearchRedaction` gebruiken:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
