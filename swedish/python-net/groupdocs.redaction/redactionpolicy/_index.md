---
title: "RedactionPolicy klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en saneringspolicy som innehåller en uppsättning specifika redigeringar att tillämpa."
type: docs
url: /sv/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Representerar en saneringspolicy som innehåller en uppsättning specifika redigeringar att tillämpa.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

RedactionPolicy‑typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Initierar en ny RedactionPolicy‑instans. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Initierar en ny RedactionPolicy med en specifik lista av redigeringar. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Läser in en RedactionPolicy från en XML‑fil. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Läser in en RedactionPolicy‑instans från en ström som innehåller XML‑konfiguration. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Sparar redigeringspolicyn till en fil. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Sparar redigeringspolicyn till en ström. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Listan över fullständigt konfigurerade [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-avledda klasser. |

### Exempel

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Bygg en återanvändbar policy i minnet
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Applicera policyn på ett dokument
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Uppgiftsguider som använder `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Se även
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
