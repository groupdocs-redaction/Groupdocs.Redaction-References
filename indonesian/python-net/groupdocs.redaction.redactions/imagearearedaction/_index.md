---
title: "kelas ImageAreaRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi yang menempatkan persegi panjang berwarna pada area tertentu dalam dokumen gambar."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Mewakili redaksi yang menempatkan persegi panjang berwarna pada area tertentu dalam dokumen gambar.

Pelajari lebih lanjut:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Tipe ImageAreaRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Menginisialisasi ImageAreaRedaction baru untuk menyensor area persegi panjang tertentu. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Menerapkan redaksi pada instance format yang diberikan. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Deskripsi redaksi, berisi nama dan parameternya. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | Opsi RegionReplacementOptions dengan parameter warna dan area. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Posisi kiri-atas area yang akan dihapus. |

### Contoh

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Panduan tugas yang menggunakan `ImageAreaRedaction`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
