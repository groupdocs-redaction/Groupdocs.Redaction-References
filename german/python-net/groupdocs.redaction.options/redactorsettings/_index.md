---
title: "Klasse RedactorSettings"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Redaktions‑Einstellungen dar, die eine Anpassung des Redaktionsprozesses ermöglichen."
type: docs
url: /de/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Stellt Redaktions‑Einstellungen dar, die eine Anpassung des Redaktionsprozesses ermöglichen.

Mehr erfahren

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Der Typ RedactorSettings stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initialisiert eine neue Instanz der Klasse RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initialisiert eine neue RedactorSettings-Instanz mit einer angegebenen ILogger-Instanz. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit einer angegebenen IRedactionCallback-Instanz. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initialisiert eine neue RedactorSettings-Instanz mit dem angegebenen IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initialisiert eine neue RedactorSettings-Instanz mit dem angegebenen Logger und Callback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initialisiert eine neue Instanz der Klasse RedactorSettings mit den angegebenen ILogger-, IRedactionCallback- und IOcrConnector-Instanzen. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Der Logger, der für das Protokollieren von Ereignissen und Fehlern verwendet wird. Muss eine Instanz einer Klasse sein, die [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) implementiert. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | Die OCR-Connector-Instanz, die [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) implementiert. |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Der Redaktions-Callback, der verwendet wird, um jede Redaktionsbeschreibung zu bewerten. |

### Beispiel

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

### Siehe auch
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
