---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru dari kelas MetadataSearchRedaction, menggunakan nilai untuk mencocokkan item yang disensor."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Menginisialisasi instance baru dari kelas MetadataSearchRedaction, menggunakan nilai untuk mencocokkan item yang disensor.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| value_pattern | `str` | Ekspresi reguler untuk mencari dan mengganti |
| replacement | `str` | Penggantian teks |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Menginisialisasi instance baru dari MetadataSearchRedaction, menggunakan nama item dan nilai untuk mencocokkan item yang disensor.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| value_pattern | `str` | Ekspresi reguler untuk mencari dan mengganti nilai item metadata. |
| replacement | `str` | Penggantian teks. |
| key_pattern | `str` | Ekspresi reguler untuk mencari dan mengganti nama item metadata. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Ganti semua alamat email yang ditemukan dalam nilai metadata
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Menginisialisasi instance baru dari kelas MetadataSearchRedaction, menggunakan nilai untuk mencocokkan item yang disensor.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| replacement | `str` | Penggantian teks. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Redaksi semua alamat email dalam metadata
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Menginisialisasi instance baru dari MetadataSearchRedaction menggunakan nama item dan nilai untuk mencocokkan item yang disensor.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti nilai item metadata. |
| replacement | `str` | Penggantian teks. |
| key_regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti nama item metadata. |

### Contoh

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Redaksi alamat email dalam nilai metadata
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Lihat Juga
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
