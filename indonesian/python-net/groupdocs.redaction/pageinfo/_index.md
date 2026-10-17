---
title: "Kelas PageInfo"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili informasi halaman singkat."
type: docs
url: /id/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Mewakili informasi halaman singkat.

Pelajari lebih lanjut:
- https://docs.groupdocs.com/redaction/net/get-file-info/

Tipe PageInfo menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | Tinggi halaman. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Nomor halaman. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | Lebar halaman. |

### Contoh

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### Lihat Juga
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
