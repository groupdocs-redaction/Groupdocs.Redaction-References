---
title: "RedactorSettings klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt redactiesettings voor, waarmee het redactieproces kan worden aangepast."
type: docs
url: /nl/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Stelt redactiesettings voor, waarmee het redactieproces kan worden aangepast.

Meer informatie

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Het type RedactorSettings bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initialiseert een nieuw RedactorSettings-exemplaar met een gegeven ILogger-instantie. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een gegeven IRedactionCallback-instantie. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initialiseert een nieuw RedactorSettings-exemplaar met de opgegeven IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initialiseert een nieuw RedactorSettings-exemplaar met de opgegeven logger en callback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met gegeven ILogger-, IRedactionCallback- en IOcrConnector-instanties. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | De logger die wordt gebruikt voor het loggen van gebeurtenissen en fouten. Moet een instantie zijn van een klasse die [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) implementeert. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | De OCR-connectorinstantie die [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) implementeert. |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | De redactiecallback die wordt gebruikt om elke redactiebeschrijving te evalueren. |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
