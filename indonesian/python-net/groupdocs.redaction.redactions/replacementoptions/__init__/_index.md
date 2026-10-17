---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru dari ReplacementOptions dengan teks pengganti yang ditentukan."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Menginisialisasi instance baru dari ReplacementOptions dengan teks pengganti yang ditentukan.

```python
def __init__(self, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| replacement | `str` | Penggantian teks. |

### Contoh

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ganti teks yang cocok dengan "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Menginisialisasi instance baru dari kelas ReplacementOptions dengan persegi panjang berwarna sebagai opsi.

```python
def __init__(self, color):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| color | `System.Drawing.Color` | Warna persegi panjang. |

### Lihat Juga
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
