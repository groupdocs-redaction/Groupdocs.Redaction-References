---
title: "Clase RedactorSettings"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa la configuración de redacción, permitiendo personalizar el proceso de redacción."
type: docs
url: /es/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Representa la configuración de redacción, permitiendo personalizar el proceso de redacción.

Aprende más

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

El tipo RedactorSettings expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Inicializa una nueva instancia de la clase RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Inicializa una nueva instancia de RedactorSettings con una instancia de ILogger dada. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Inicializa una nueva instancia de la clase RedactorSettings con una instancia de IRedactionCallback dada. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Inicializa una nueva instancia de RedactorSettings con el IOcrConnector especificado. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Inicializa una nueva instancia de RedactorSettings con el logger y la devolución de llamada especificados. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Inicializa una nueva instancia de la clase RedactorSettings con instancias dadas de ILogger, IRedactionCallback y IOcrConnector. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | El logger usado para registrar eventos y errores. Debe ser una instancia de una clase que implemente [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | La instancia del conector OCR que implementa [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | La devolución de llamada de redacción usada para evaluar cada descripción de redacción. |

### Ejemplo

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

### Ver también
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
