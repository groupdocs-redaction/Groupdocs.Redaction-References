---
title: "Kelas PageAreaRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi tekstual kompleks yang memengaruhi teks, gambar, dan anotasi dalam area halaman."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Mewakili redaksi tekstual kompleks yang memengaruhi teks, gambar, dan anotasi dalam area halaman.

Pelajari lebih lanjut

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

Tipe PageAreaRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Menginisialisasi instance PageAreaRedaction baru. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Menginisialisasi PageAreaRedaction baru. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Menerapkan redaksi pada instance format yang diberikan. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | Opsi RegionReplacementOptions dengan parameter warna dan area. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Instance [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) yang menentukan jenis penggantian teks. (diturunkan dari [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Deskripsi penyensoran, berisi nama dan parameternya. (diturunkan dari [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Implementasi IOcrConnector yang digunakan untuk mengekstrak teks dari konten grafis. (diturunkan dari [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Pola ekspresi reguler yang digunakan untuk pencocokan. (diturunkan dari [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
