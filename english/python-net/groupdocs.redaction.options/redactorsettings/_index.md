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

- More details about implementing ILogger interface: https://docs.groupdocs.com/redaction/python-net/use-advanced-logging/
- More details about implementing IRedactionCallback interface: https://docs.groupdocs.com/redaction/python-net/use-redaction-callback/

The RedactorSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Initializes a new instance of the RedactorSettings class. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Initializes a new RedactorSettings instance with the specified logger. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Initializes a new RedactorSettings instance with a given IRedactionCallback implementation. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Initializes a new RedactorSettings instance with the specified IOcrConnector. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Initializes a new [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/) instance with optional logger, callback, and OCR connector. |

### Properties
| Property | Description |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | The logger used for logging events and errors. It must implement [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | The OCR connector used to recognize text in images, which must implement [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | The redaction callback that implements [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) and is invoked for each redaction. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, RedactorSettings
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

class RedactionDump:
    def accept_redaction(self, description):
        print(f"{description.redaction_type.name} redaction, {description.action_type.name} action, item {description.original_text}.")
        if description.replacement is not None:
            print(f"Text {description.replacement.original_text} is replaced with {description.replacement.replacement}.")
        return True

settings = RedactorSettings(RedactionDump())
with Redactor("./sample.docx", LoadOptions(), settings) as redactor:
    redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions("[personal]")))
    result_path = redactor.save()
    print("Document redacted. Output saved to", result_path)
```

### Guides
Task guides that use `RedactorSettings`:

* [Use redaction callback](/redaction/python-net/guides/use-redaction-callback/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
