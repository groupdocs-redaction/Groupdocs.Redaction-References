---
title: "RemovePageRedaction-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en radering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Representerar en radering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument.

Läs mer
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction-typen visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Initierar en ny RemovePageRedaction. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Tillämpa redigeringen på en given formatinstans. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Antalet sidor att ta bort. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Startpositionsindexet (0-baserat). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Sökreferenspositionen, antingen början eller slutet av ett dokument. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Beskrivningen av raderingen, som innehåller dess namn och parametrar. (ärvd från [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Ta bort 1 sida räknat från dokumentets slut
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Applicera maskeringen
        result = redactor.apply(rem_opt)

        # Spara det redigerade dokumentet
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Uppgiftsguider som använder `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Se även
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
