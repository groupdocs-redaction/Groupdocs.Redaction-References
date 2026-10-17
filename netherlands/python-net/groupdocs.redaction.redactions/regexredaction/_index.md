---
title: "RegexRedaction‑klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een tekstredactie voor die tekst in het document zoekt en vervangt door de opgegeven reguliere expressie te matchen."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Stelt een tekstredactie voor die tekst in het document zoekt en vervangt door de opgegeven reguliere expressie te matchen.

Meer informatie

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Het type RegexRedaction geeft de volgende leden weer:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Initialiseert een nieuw exemplaar van RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Initialiseert een nieuw RegexRedaction‑exemplaar. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | De beschrijving van de redactie, met de naam en parameters. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Het reguliere expressiepatroon dat wordt gebruikt voor overeenstemming. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | De [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)‑instantie die het type tekstvervanging specificeert. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | De IOcrConnector‑implementatie die wordt gebruikt om tekst uit grafische inhoud te extraheren. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # vervang met tekst
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # vervang met blauwe vaste rechthoek
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Taakgidsen die `RegexRedaction` gebruiken:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
