---
title: "RedactorSettings क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "रेडैक्शन सेटिंग्स को दर्शाता है, जिससे रेडैक्शन प्रक्रिया को अनुकूलित किया जा सकता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

रेडैक्शन सेटिंग्स को दर्शाता है, जिससे रेडैक्शन प्रक्रिया को अनुकूलित किया जा सकता है।

और अधिक जानें

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

RedactorSettings प्रकार निम्नलिखित सदस्य उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | दिए गए ILogger इंस्टेंस के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | दिए गए IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | निर्दिष्ट IOcrConnector के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | निर्दिष्ट लॉगर और कॉलबैक के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | दिए गए ILogger, IRedactionCallback और IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | इवेंट और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला लॉगर। यह [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) को लागू करने वाली क्लास का इंस्टेंस होना चाहिए। |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) को लागू करने वाला OCR कनेक्टर इंस्टेंस। |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | प्रत्येक रेडैक्शन विवरण का मूल्यांकन करने के लिए उपयोग किया जाने वाला रेडैक्शन कॉलबैक। |

### उदाहरण

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

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
