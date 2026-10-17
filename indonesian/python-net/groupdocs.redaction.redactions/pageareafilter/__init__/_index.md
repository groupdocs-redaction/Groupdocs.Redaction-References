---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi PageAreaFilter baru untuk menyensor area tertentu."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Menginisialisasi PageAreaFilter baru untuk menyensor area tertentu.

```python
def __init__(self, top_left, size):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinat area kiri-atas. |
| size | `System.Drawing.Size` | Ukuran area dan warna. |

### Contoh

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Lihat Juga
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
