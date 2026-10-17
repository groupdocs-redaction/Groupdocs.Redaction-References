---
title: "kelas RemovePageRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi yang menghapus halaman (slide, lembar kerja, dll.) dari dokumen."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Mewakili redaksi yang menghapus halaman (slide, lembar kerja, dll.) dari dokumen.

Pelajari lebih lanjut
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Tipe RemovePageRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Menginisialisasi RemovePageRedaction baru. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Menerapkan redaksi pada instance format yang diberikan. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Jumlah halaman yang akan dihapus. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Indeks posisi awal (berbasis 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Posisi referensi pencarian, baik awal maupun akhir dokumen. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Deskripsi redaksi, berisi nama dan parameternya. (diturunkan dari [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Hapus 1 halaman menghitung dari akhir dokumen
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(rem_opt)

        # Simpan dokumen yang telah di‑redact
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Panduan tugas yang menggunakan `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
