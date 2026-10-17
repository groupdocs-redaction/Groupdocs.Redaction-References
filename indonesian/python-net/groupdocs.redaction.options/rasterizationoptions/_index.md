---
title: "kelas RasterizationOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyediakan opsi untuk mengonversi file menjadi PDF."
type: docs
url: /id/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Menyediakan opsi untuk mengonversi file menjadi PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Tipe RasterizationOptions menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Menginisialisasi sebuah instance baru. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Mendaftarkan opsi rasterisasi lanjutan untuk diterapkan. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Mendaftarkan opsi rasterisasi lanjutan untuk diterapkan. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Tingkat kepatuhan PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Bendera enabled menunjukkan apakah semua halaman dalam dokumen dikonversi menjadi gambar dan ditempatkan dalam satu file PDF. True secara default; set ke False untuk menghindari rasterisasi. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Indikator bernilai True jika opsi rasterisasi lanjutan diatur. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Jumlah halaman yang akan dikonversi menjadi PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | Indeks halaman pertama (berbasis 0) untuk dikonversi menjadi PDF. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### Lihat Juga
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
