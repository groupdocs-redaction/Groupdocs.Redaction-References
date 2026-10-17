---
title: "Kelas IDocumentInfo"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyediakan metode yang diperlukan untuk mendapatkan informasi dasar dokumen."
type: docs
url: /id/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Menyediakan metode yang diperlukan untuk mendapatkan informasi dasar dokumen.

Pelajari lebih lanjut: Dapatkan info file (https://docs.groupdocs.com/redaction/net/get-file-info/).

Tipe IDocumentInfo menampilkan anggota-anggota berikut:

### Properti
| Properti | Deskripsi |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Deskripsi format file. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Jumlah total halaman. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Daftar objek [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) yang mewakili informasi halaman. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Ukuran dokumen dalam byte. |

### Contoh

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Lihat Juga
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
