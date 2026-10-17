---
title: "Classe RedactorSettings"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta le impostazioni di redazione, consentendo di personalizzare il processo di redazione."
type: docs
url: /it/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Rappresenta le impostazioni di redazione, consentendo di personalizzare il processo di redazione.

Per saperne di più

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Il tipo RedactorSettings espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Inizializza una nuova istanza della classe RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Inizializza una nuova istanza di RedactorSettings con una data istanza di ILogger. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Inizializza una nuova istanza della classe RedactorSettings con una data istanza di IRedactionCallback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Inizializza una nuova istanza di RedactorSettings con l'IOcrConnector specificato. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Inizializza una nuova istanza di RedactorSettings con il logger e il callback specificati. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Inizializza una nuova istanza della classe RedactorSettings con le istanze di ILogger, IRedactionCallback e IOcrConnector fornite. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Il logger utilizzato per registrare eventi ed errori. Deve essere un'istanza di una classe che implementa [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | L'istanza del connettore OCR che implementa [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Il callback di redazione utilizzato per valutare ogni descrizione di redazione. |

### Esempio

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

### Vedi anche
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
