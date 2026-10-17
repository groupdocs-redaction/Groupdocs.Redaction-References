---
title: "Kelas RegionReplacementOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili parameter warna dan area untuk penggantian wilayah gambar."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Mewakili parameter warna dan area untuk penggantian wilayah gambar.

Pelajari lebih lanjut:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Tipe RegionReplacementOptions menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Menginisialisasi sebuah instance RegionReplacementOptions baru. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Menginisialisasi sebuah instance baru dari kelas RegionReplacementOptions yang ukurannya cocok dengan teks yang diberikan. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Warna yang digunakan untuk mengisi area yang disensor. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Lebar dan tinggi persegi panjang. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Tentukan posisi kiri‑atas area yang akan diganti
    point = Point(516, 311)
    # Tentukan ukuran area yang akan diganti
    size = Size(170, 35)
    # Gunakan persegi panjang hitam solid sebagai pengganti
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Panduan tugas yang menggunakan `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
