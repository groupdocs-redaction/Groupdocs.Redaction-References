---
title: "ExactPhraseRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en textmaskering som ersätter en exakt fras i dokumentets text, skiftlägesokänslig som standard."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Representerar en textmaskering som ersätter en exakt fras i dokumentets text, skiftlägesokänslig som standard.

Läs mer:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction-typen visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initierar en ny instans av ExactPhraseRedaction i läge utan hänsyn till skiftläge. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initierar en ny ExactPhraseRedaction-instans. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Tillämpa redigeringen på en given formatinstans. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | Beskrivningen av redigeringen, som innehåller redigeringsnamnet och parametrarna. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Värdet som indikerar om sökningen är skiftlägeskänslig. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Flaggan för textriktning som indikerar om texten är från höger till vänster. Standardvärdet är False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | Strängen att söka i och ersätta. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Instansen [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) som specificerar typen av textersättning. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Implementeringen av IOcrConnector som används för att extrahera text från grafiskt innehåll. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # skiftlägeskänslig ersättning
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Uppgiftsguider som använder `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
