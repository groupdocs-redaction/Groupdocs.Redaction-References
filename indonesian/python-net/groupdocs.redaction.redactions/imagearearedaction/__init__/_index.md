---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi ImageAreaRedaction baru untuk menyensor area persegi panjang tertentu."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Menginisialisasi ImageAreaRedaction baru untuk menyensor area persegi panjang tertentu.

```python
def __init__(self, top_left, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Koordinat area kiri-atas. |
| options | `RegionReplacementOptions` | Ukuran area dan warna. |

### Contoh

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Tentukan sudut kiri-atas area yang akan disensor
top_left = Point(385, 485)
# Tentukan ukuran dan warna wilayah penyensoran
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Buat objek penyensoran
redaction = ImageAreaRedaction(top_left, region_options)
```

### Lihat Juga
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
