---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, dengan pengaturan untuk menghapus semua anotasi (mencocokkan semua)."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, dengan pengaturan untuk menghapus semua anotasi (mencocokkan semua).

```python
def __init__(self):
    ...
```

### Contoh

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Hapus semua anotasi
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, menghapus anotasi yang cocok dengan ekspresi yang diberikan.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| pattern | `str` | Ekspresi reguler. |

### Contoh

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Hapus anotasi yang berisi kata "internal" (tidak peka huruf).
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, menghapus anotasi yang cocok dengan ekspresi yang diberikan.

```python
def __init__(self, regex):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler. |

### Contoh

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Hapus anotasi yang isinya cocok dengan regex (tidak peka huruf besar/kecil)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Lihat Juga
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
