---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir dosya yolu kullanarak yeni bir Redactor örneği başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Bir dosya yolu kullanarak yeni bir Redactor örneği başlatır.

```python
def __init__(self, file_path):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_path | `str` | Dosyanın yolu. |

### Örnek

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Burada redaksiyon işlemlerini gerçekleştirin
    pass
```

## __init__ {#document}

`[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` kullanarak bir akış ile yeni bir örnek başlatır.

```python
def __init__(self, document):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| document | `io.RawIOBase` | Belgenin kaynak akışı. |

### Örnek

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Belgeyi ikili akış olarak açın
    with open("./sample.pdf", "rb") as stream:
        # Belgeyi akıştan yükleyin
        with Redactor(stream) as redactor:
            # Burada redaksiyonları gerçekleştirin
            pass
```

## __init__ {#file_path-load_options}

`[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` şifre korumalı belge için yolunu kullanarak yeni bir örnek başlatır.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_path | `str` | Dosyanın yolu. |
| load_options | `LoadOptions` | Şifre dahil seçenekler. |

### Örnek

```python
from groupdocs.redaction import Redactor

# Bir dosya yolundan şifre korumalı belgeyi yükle
with Redactor("protected.docx") as redactor:
    # Burada redaksiyon işlemlerini gerçekleştirin
    pass
```

## __init__ {#file_path-load_options-settings}

Şifre korumalı bir belge için yol ve ayarları kullanarak yeni bir Redactor örneği başlatır.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_path | `str` | Dosya yolu. |
| load_options | `LoadOptions` | Şifre dahil dosya bağımlı seçenekler. |
| settings | `RedactorSettings` | Redaksiyon süreci için varsayılan ayarlar. |

### Örnek

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Şifre korumalı bir belge için bir akış kullanarak yeni bir Redactor örneği başlatır.

```python
def __init__(self, document, load_options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| document | `io.RawIOBase` | Kaynak giriş akışı. |
| load_options | `LoadOptions` | Şifre dahil seçenekler. |

### Örnek

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Korunan PDF'yi ikili akış olarak aç
    with open(r"C:\sample.pdf", "rb") as stream:
        # Şifreyi LoadOptions aracılığıyla sağlayın
        load_options = LoadOptions("mypassword")
        # Redactor'ı akış ve yükleme seçenekleriyle başlat
        with Redactor(stream, load_options) as redactor:
            # Burada redaksiyon işlemlerini gerçekleştirin
            pass
```

## __init__ {#document-load_options-settings}

`[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` şifre korumalı bir belge için bir akış ve ayarları kullanarak yeni bir örnek başlatır.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| document | `io.RawIOBase` | Kaynak giriş akışı. |
| load_options | `LoadOptions` | Şifre dahil seçenekler. |
| settings | `RedactorSettings` | Kırpma işlemi için varsayılan ayarlar. |

### Ayrıca Bakınız
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
