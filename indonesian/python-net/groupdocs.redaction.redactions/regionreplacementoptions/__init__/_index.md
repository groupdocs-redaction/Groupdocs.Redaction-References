---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi sebuah instance RegionReplacementOptions baru."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Menginisialisasi sebuah instance RegionReplacementOptions baru.

```python
def __init__(self, fill_color, size):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Warna untuk mengisi area. |
| size | `System.Drawing.Size` | Ukuran area yang terisi. |

### Contoh

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Menginisialisasi sebuah instance baru dari kelas RegionReplacementOptions yang ukurannya cocok dengan teks yang diberikan.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Warna untuk mengisi area. |
| font | `System.Drawing.Font` | Font teks yang diharapkan. |
| expected_text | `str` | Teks yang diharapkan. |

### Lihat Juga
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
