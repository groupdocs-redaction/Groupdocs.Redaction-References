---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيلًا جديدًا لفئة RedactorSettings."
type: docs
url: /ar/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

يُنشئ مثيلًا جديدًا لفئة RedactorSettings.

```python
def __init__(self):
    ...
```

### مثال

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

يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام مثيل ILogger معين.

```python
def __init__(self, logger):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| logger | `ILogger` | مثال على فئة تُنفّذ الواجهة `ILogger`. |

## __init__ {#callback}

يُنشئ مثيلًا جديدًا لفئة RedactorSettings باستخدام مثيل IRedactionCallback معين.

```python
def __init__(self, callback):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| callback | `IRedactionCallback` | مثال على فئة تُنفّذ واجهة IRedactionCallback. |

### مثال

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

يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام IOcrConnector المحدد.

```python
def __init__(self, ocr_connector):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | تنفيذ صالح لواجهة IOcrConnector. |

## __init__ {#logger-callback}

يُنشئ مثيلًا جديدًا من RedactorSettings باستخدام logger المحدد والرد الندائي.

```python
def __init__(self, logger, callback):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| logger | `ILogger` | مثال على فئة تُنفّذ الواجهة ILogger. |
| callback | `IRedactionCallback` | مثال على فئة تنفذ واجهة IRedactionCallback. |

### مثال

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

يُنشئ مثيلًا جديدًا لفئة RedactorSettings باستخدام مثيلات ILogger و IRedactionCallback و IOcrConnector المعطاة.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| logger | `ILogger` | مثال على فئة تنفذ واجهة `ILogger`. |
| callback | `IRedactionCallback` | مثال على فئة تنفذ واجهة `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | مثال على تنفيذ واجهة `IOcrConnector`. يمكن أن يكون `None`. |

### مثال

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### انظر أيضًا
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
