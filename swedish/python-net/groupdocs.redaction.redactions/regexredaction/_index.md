---
title: "Klassen RegexRedaction"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en textradering som söker och ersätter text i dokumentet genom att matcha angivet reguljärt uttryck."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Representerar en textradering som söker och ersätter text i dokumentet genom att matcha angivet reguljärt uttryck.

Läs mer

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Typen RegexRedaction exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Initierar en ny instans av RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Initierar en ny RegexRedaction-instans. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Tillämpa redigeringen på en given formatinstans. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Beskrivningen av redigeringen, som innehåller dess namn och parametrar. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Det reguljära uttrycksmönstret som används för matchning. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Instansen [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) som specificerar typen av textersättning. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Implementeringen av IOcrConnector som används för att extrahera text från grafiskt innehåll. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # ersätt med text
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # ersätt med blå solid rektangel
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Uppgiftsguider som använder `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
