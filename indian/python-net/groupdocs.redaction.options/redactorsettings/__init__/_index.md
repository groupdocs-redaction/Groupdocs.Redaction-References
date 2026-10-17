---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self):
    ...
```

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

## __init__ {#logger}

दिए गए ILogger इंस्टेंस के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, logger):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| logger | `ILogger` | एक क्लास का इंस्टेंस जो `ILogger` इंटरफ़ेस को लागू करता है। |

## __init__ {#callback}

दिए गए IRedactionCallback इंस्टेंस के साथ RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, callback):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| callback | `IRedactionCallback` | एक क्लास का इंस्टेंस जो IRedactionCallback इंटरफ़ेस को लागू करता है। |

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

## __init__ {#ocr_connector}

निर्दिष्ट IOcrConnector के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, ocr_connector):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | IOcrConnector इंटरफ़ेस की एक वैध कार्यान्वयन। |

## __init__ {#logger-callback}

निर्दिष्ट लॉगर और कॉलबैक के साथ नया RedactorSettings इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, logger, callback):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| logger | `ILogger` | एक क्लास का इंस्टेंस जो ILogger इंटरफ़ेस को लागू करता है। |
| callback | `IRedactionCallback` | IRedactionCallback इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |

### उदाहरण

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

दिए गए ILogger, IRedactionCallback और IOcrConnector इंस्टेंस के साथ RedactorSettings क्लास का नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |
| callback | `IRedactionCallback` | `IRedactionCallback` इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |
| ocr_connector | `IOcrConnector` | `IOcrConnector` इंटरफ़ेस कार्यान्वयन का एक उदाहरण। यह `None` हो सकता है। |

### उदाहरण

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### संबंधित देखें
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
