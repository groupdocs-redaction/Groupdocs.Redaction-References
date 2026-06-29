---
title: RedactorSettings class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents redaction settings, allowing to customize the redaction process."
type: docs
url: /python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Represents redaction settings, allowing to customize the redaction process.

Learn more

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

The RedactorSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initializes a new instance of the RedactorSettings class. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initializes a new RedactorSettings instance with a given ILogger instance. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initializes a new RedactorSettings instance with the specified IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initializes a new RedactorSettings instance with the specified logger and callback. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances. |

### Properties
| Property | Description |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | The logger used for logging events and errors. Must be an instance of a class implementing [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | The OCR connector instance implementing [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | The redaction callback used to evaluate each redaction description. |

### Example

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

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
