---
title: "Kelas PreviewOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau."
type: docs
url: /id/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau.

Kelas ini memungkinkan penentuan format pratinjau, dimensi gambar, nomor halaman, dan delegasi yang membuat serta secara opsional melepaskan aliran untuk setiap halaman yang dihasilkan.

Tipe PreviewOptions menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Menginisialisasi instance PreviewOptions baru. Aliran output akan ditutup setelah digunakan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Menginisialisasi instance PreviewOptions baru, menyebabkan aliran output dikembalikan ke klien untuk penggunaan lebih lanjut. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Delegate pembuatan aliran halaman. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Tinggi pratinjau halaman. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Nomor halaman untuk menghasilkan pratinjau. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Format gambar pratinjau. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Delegate penyelesaian pratinjau halaman. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Lebar pratinjau halaman. |

### Contoh

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Buat file untuk gambar pratinjau halaman yang diberikan
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Lihat Juga
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
