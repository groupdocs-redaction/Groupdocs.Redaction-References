---
title: "Kelas PageAreaFilter"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili filter redaksi, mengatur area dalam halaman dokumen untuk menerapkan redaksi."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Mewakili filter redaksi, mengatur area dalam halaman dokumen untuk menerapkan redaksi.

Pelajari lebih lanjut

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Tipe PageAreaFilter menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Menginisialisasi PageAreaFilter baru untuk menyensor area tertentu. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Persegi panjang (posisi kiri-atas dan ukuran area) pada halaman. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
