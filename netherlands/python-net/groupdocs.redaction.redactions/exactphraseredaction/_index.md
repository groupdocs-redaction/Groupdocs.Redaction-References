---
title: "ExactPhraseRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een tekstredactie voor die een exacte zin in de tekst van het document vervangt, standaard niet-hoofdlettergevoelig."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Stelt een tekstredactie voor die een exacte zin in de tekst van het document vervangt, standaard niet-hoofdlettergevoelig.

Meer informatie:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Het ExactPhraseRedaction type maakt de volgende leden beschikbaar:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initialiseert een nieuw exemplaar van ExactPhraseRedaction in hoofdletterongevoelige modus. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initialiseert een nieuw ExactPhraseRedaction exemplaar. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | De beschrijving van de redactie, met de naam van de redactie en parameters. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | De waarde die aangeeft of de zoekopdracht hoofdlettergevoelig is. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | De tekstrichtingsvlag die aangeeft of de tekst van rechts naar links loopt. Standaard is False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | De tekenreeks om te zoeken en te vervangen. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | De [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)‑instantie die het type tekstvervanging specificeert. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | De IOcrConnector‑implementatie die wordt gebruikt om tekst uit grafische inhoud te extraheren. (geërfd van [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # hoofdlettergevoelige vervanging
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Taakgidsen die `ExactPhraseRedaction` gebruiken:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
