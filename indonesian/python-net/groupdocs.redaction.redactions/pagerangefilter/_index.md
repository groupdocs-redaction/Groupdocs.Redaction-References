---
title: "Kelas PageRangeFilter"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili filter redaksi, mengatur rentang halaman dalam dokumen untuk menerapkan redaksi."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Mewakili filter redaksi, mengatur rentang halaman dalam dokumen untuk menerapkan redaksi.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Tipe PageRangeFilter menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Menginisialisasi RemovePageRedaction baru. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Jumlah halaman yang akan dihapus. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Indeks posisi awal (berbasis 0). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Posisi referensi pencarian, baik awal maupun akhir dokumen. |

### Contoh

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Mendefinisikan filter yang menargetkan halaman terakhir dan halaman sebelumnya
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Filter dapat digabungkan dengan filter lain, misalnya PageAreaFilter,
# dan diteruskan ke ReplacementOptions.Filters saat mengonfigurasi redaksi.
```

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
