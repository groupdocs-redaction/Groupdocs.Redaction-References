---
title: "PageAreaRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een complexe tekstuele redactie voor die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Stelt een complexe tekstuele redactie voor die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt.

Meer informatie

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

Het type PageAreaRedaction exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Initialiseert een nieuwe PageAreaRedaction‑instantie. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Initialiseert een nieuwe PageAreaRedaction. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | De RegionReplacementOptions‑opties met kleur- en gebiedsparameters. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | De [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)‑instantie die het type tekstvervanging specificeert. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | De beschrijving van de redactie, met de naam en parameters. (geërfd van [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | De IOcrConnector‑implementatie die wordt gebruikt om tekst uit grafische inhoud te extraheren. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Het regex‑patroon dat wordt gebruikt voor matching. (geërfd van [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
