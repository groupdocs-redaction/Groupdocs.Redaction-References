---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru dari RegexRedaction."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Menginisialisasi instance baru dari RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| pattern | `str` | Ekspresi reguler untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |

### Contoh

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Menginisialisasi instance RegexRedaction baru.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |

### Contoh

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Lihat Juga
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
