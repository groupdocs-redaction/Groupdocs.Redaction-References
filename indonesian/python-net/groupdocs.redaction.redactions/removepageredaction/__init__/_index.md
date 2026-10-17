---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi RemovePageRedaction baru."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Menginisialisasi RemovePageRedaction baru.

```python
def __init__(self, origin, index, count):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Cari posisi referensi, awal atau akhir dokumen. |
| index | `int` | Indeks posisi mulai (berbasis 0). |
| count | `int` | Jumlah halaman yang akan dihapus. |

### Contoh

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Hapus 3 halaman mulai dari halaman kedua (indeks berbasis 0 = 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Lihat Juga
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
