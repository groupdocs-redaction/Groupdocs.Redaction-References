---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru dari kelas RedactorSettings."
type: docs
url: /id/python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi instance baru dari kelas RedactorSettings.

```python
def __init__(self):
    ...
```

### Contoh

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

Menginisialisasi instance RedactorSettings baru dengan instance ILogger yang diberikan.

```python
def __init__(self, logger):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| logger | `ILogger` | Sebuah instance dari kelas yang mengimplementasikan antarmuka `ILogger`. |

## __init__ {#callback}

Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IRedactionCallback yang diberikan.

```python
def __init__(self, callback):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| callback | `IRedactionCallback` | Sebuah instance dari kelas yang mengimplementasikan antarmuka IRedactionCallback. |

### Contoh

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

Menginisialisasi instance RedactorSettings baru dengan IOcrConnector yang ditentukan.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| ocr_connector | `IOcrConnector` | Implementasi IOcrConnector yang valid. |

## __init__ {#logger-callback}

Menginisialisasi instance RedactorSettings baru dengan logger dan callback yang ditentukan.

```python
def __init__(self, logger, callback):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| logger | `ILogger` | Sebuah instance dari kelas yang mengimplementasikan antarmuka ILogger. |
| callback | `IRedactionCallback` | Sebuah instance dari kelas yang mengimplementasikan antarmuka IRedactionCallback. |

### Contoh

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

## __init__ {#logger-callback-ocr_connector}

Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger, IRedactionCallback, dan IOcrConnector yang diberikan.

```python
def __init__(self, logger, callback, ocr_connector):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| logger | `ILogger` | Sebuah instance dari kelas yang mengimplementasikan antarmuka `ILogger`. |
| callback | `IRedactionCallback` | Sebuah instance dari kelas yang mengimplementasikan antarmuka `IRedactionCallback`. |
| ocr_connector | `IOcrConnector` | Sebuah instance dari implementasi antarmuka `IOcrConnector`. Bisa berupa `None`. |

### Contoh

```python
from groupdocs.redaction.options import RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

settings = RedactorSettings(callback=accept)
```

### Lihat Juga
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/)
