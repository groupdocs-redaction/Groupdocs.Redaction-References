---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance PreviewOptions baru."
type: docs
url: /id/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Menginisialisasi instance PreviewOptions baru. Aliran output akan ditutup setelah digunakan.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Membuat aliran untuk pratinjau halaman tertentu. |

## __init__ {#create_page_stream-release_page_stream}

Menginisialisasi instance PreviewOptions baru, menyebabkan aliran output dikembalikan ke klien untuk penggunaan lebih lanjut.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Membuat aliran untuk pratinjau halaman tertentu. |
| release_page_stream | `ReleasePageStream` | Memberitahukan bahwa pembuatan pratinjau halaman selesai dan mendapatkan aliran keluaran. |

### Lihat Juga
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
