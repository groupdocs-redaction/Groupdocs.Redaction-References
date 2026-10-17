---
title: "PageAreaRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en komplex textuell radering som påverkar text, bilder och annotationer i ett område på sidan."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Representerar en komplex textuell radering som påverkar text, bilder och annotationer i ett område på sidan.

Läs mer

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Initierar en ny PageAreaRedaction-instans. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Initierar en ny PageAreaRedaction. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Tillämpa redigeringen på en given formatinstans. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | RegionReplacementOptions-alternativen med färg- och områdesparametrar. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Instansen [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) som specificerar typen av textersättning. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Beskrivningen av raderingen, som innehåller dess namn och parametrar. (ärvd från [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Implementeringen av IOcrConnector som används för att extrahera text från grafiskt innehåll. (ärvd från [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Det reguljära uttrycksmönstret som används för matchning. (ärvd från [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
