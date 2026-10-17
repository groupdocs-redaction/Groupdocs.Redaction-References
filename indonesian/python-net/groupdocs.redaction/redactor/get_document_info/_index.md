---
title: "metode get_document_info"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mengambil informasi umum tentang dokumen, seperti ukuran dan jumlah halaman."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Mengambil informasi umum tentang dokumen, seperti ukuran dan jumlah halaman.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Menaikkan | Deskripsi |
| :- | :- |
| `PasswordRequiredException` | Dilempar ketika dokumen dilindungi kata sandi. |
| `IncorrectPasswordException` | Dilempar ketika kata sandi yang diberikan tidak valid. |

### Contoh

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Lihat Juga
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
