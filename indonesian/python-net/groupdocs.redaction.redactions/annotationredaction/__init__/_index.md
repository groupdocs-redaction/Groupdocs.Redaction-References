---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi AnnotationRedaction baru dengan pola regex dan teks pengganti."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Menginisialisasi AnnotationRedaction baru dengan pola regex dan teks pengganti.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| pattern | `str` | Ekspresi reguler untuk mencocokkan. |
| replacement | `str` | Penggantian tekstual untuk teks yang cocok. |

### Contoh

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Saring kata "approved" dalam teks anotasi
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Menginisialisasi instance baru dari [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencocokkan. |
| replacement | `str` | Penggantian tekstual untuk teks yang cocok. |

### Contoh

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Saring kata "approved" (tidak peka huruf) dan ganti dengan "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Lihat Juga
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
