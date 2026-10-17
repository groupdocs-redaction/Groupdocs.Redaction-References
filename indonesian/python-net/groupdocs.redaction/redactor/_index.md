---
title: "Kelas Redactor"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili kelas utama yang mengontrol proses redaksi dokumen, memungkinkan membuka, meredaksi, dan menyimpan dokumen."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Mewakili kelas utama yang mengontrol proses redaksi dokumen, memungkinkan membuka, meredaksi, dan menyimpan dokumen.

Pelajari lebih lanjut
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Tipe Redactor menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Menginisialisasi instance Redactor baru menggunakan jalur file. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) menggunakan aliran. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Menginisialisasi instance Redactor baru untuk dokumen yang dilindungi kata sandi menggunakan jalur dan pengaturannya. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Menginisialisasi instance Redactor baru untuk dokumen yang dilindungi kata sandi menggunakan aliran. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Menerapkan redaksi pada dokumen. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Menerapkan sekumpulan redaksi pada dokumen. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Menerapkan kebijakan redaksi pada dokumen. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Melepaskan sumber daya. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Menghasilkan gambar pratinjau dari halaman tertentu dalam format gambar yang diberikan. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Mengambil informasi umum tentang dokumen, seperti ukuran dan jumlah halaman. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Menyimpan dokumen ke file. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Menyimpan dokumen ke aliran, termasuk lokasi khusus. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Buka dokumen dan hapus halaman pertama
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Panduan tugas yang menggunakan `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Lihat Juga
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
