---
title: "Klassen RedactorSettings"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar redigeringsinställningar, vilket möjliggör anpassning av redigeringsprocessen."
type: docs
url: /sv/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Representerar redigeringsinställningar, vilket möjliggör anpassning av redigeringsprocessen.

Läs mer

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Typen RedactorSettings visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initierar en ny instans av klassen RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initierar en ny RedactorSettings-instans med en given ILogger-instans. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initierar en ny instans av klassen RedactorSettings med en given IRedactionCallback-instans. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initierar en ny RedactorSettings-instans med den angivna IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initierar en ny RedactorSettings-instans med den angivna logger och callback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initierar en ny instans av klassen RedactorSettings med givna ILogger-, IRedactionCallback- och IOcrConnector-instans. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Loggern som används för att logga händelser och fel. Måste vara en instans av en klass som implementerar [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | OCR‑anslutningsinstansen som implementerar [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Redigerings‑callbacken som används för att utvärdera varje redigeringsbeskrivning. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### Se även
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
