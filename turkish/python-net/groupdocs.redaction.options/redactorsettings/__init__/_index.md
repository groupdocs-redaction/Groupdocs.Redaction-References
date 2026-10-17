---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "RedactorSettings sınıfının yeni bir örneğini başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

RedactorSettings sınıfının yeni bir örneğini başlatır.

```python
def __init__(self):
    ...
```

### Örnek

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

Verilen bir ILogger örneği ile yeni bir RedactorSettings örneği başlatır.

```python
def __init__(self, logger):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` arabirimini uygulayan bir sınıfın örneği. |

## __init__ {#callback}

Verilen bir IRedactionCallback örneği ile RedactorSettings sınıfının yeni bir örneğini başlatır.

```python
def __init__(self, callback):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| callback | `IRedactionCallback` | IRedactionCallback arabirimini uygulayan bir sınıfın örneği. |

### Örnek

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

Belirtilen IOcrConnector ile yeni bir RedactorSettings örneği başlatır.

```python
def __init__(self, ocr_connector):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | IOcrConnector arabiriminin geçerli bir uygulaması. |

## __init__ {#logger-callback}

Belirtilen logger ve geri çağırma ile yeni bir RedactorSettings örneği başlatır.

```python
def __init__(self, logger, callback):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| logger | `ILogger` | ILogger arabirimini uygulayan bir sınıfın örneği. |
| callback | `IRedactionCallback` | IRedactionCallback arayüzünü uygulayan bir sınıf örneği. |

### Örnek

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Verilen ILogger, IRedactionCallback ve IOcrConnector örnekleriyle RedactorSettings sınıfının yeni bir örneğini başlatır.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| logger | `ILogger` | `ILogger` arayüzünü uygulayan bir sınıf örneği. |
| callback | `IRedactionCallback` | `IRedactionCallback` arayüzünü uygulayan bir sınıf örneği. |
| ocr_connector | `IOcrConnector` | `IOcrConnector` arayüzü uygulamasının bir örneği. `None` olabilir. |

### Örnek

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Ayrıca Bakınız
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
