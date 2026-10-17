---
title: "Classe RedactorSettings"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente les paramètres de censure, permettant de personnaliser le processus de censure."
type: docs
url: /fr/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Représente les paramètres de censure, permettant de personnaliser le processus de censure.

En savoir plus

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Le type RedactorSettings expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initialise une nouvelle instance de la classe RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initialise une nouvelle instance de RedactorSettings avec une instance ILogger donnée. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance IRedactionCallback donnée. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initialise une nouvelle instance de RedactorSettings avec le IOcrConnector spécifié. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initialise une nouvelle instance de RedactorSettings avec le logger et le rappel spécifiés. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger, IRedactionCallback et IOcrConnector fournies. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Le logger utilisé pour consigner les événements et les erreurs. Doit être une instance d’une classe implémentant [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | L’instance du connecteur OCR implémentant [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Le rappel de rédaction utilisé pour évaluer chaque description de rédaction. |

### Exemple

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

### Voir aussi
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
