---
title: "metode generate_preview"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menghasilkan gambar pratinjau dari halaman tertentu dalam format gambar yang diberikan."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Menghasilkan gambar pratinjau dari halaman tertentu dalam format gambar yang diberikan.

Pratinjau dihasilkan sesuai dengan pengaturan yang didefinisikan dalam `preview_options`, yang mencakup format gambar, dimensi, rentang halaman, dan callback untuk membuat serta melepaskan aliran halaman.

```python
def generate_preview(self, preview_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Properti gambar dan pengaturan rentang halaman. |

### Contoh

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Mengembalikan aliran file yang dapat ditulis untuk gambar pratinjau dari halaman yang diberikan.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Dipanggil setelah gambar pratinjau selesai ditulis.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Lihat Juga
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
