---
title: "get_supported_file_types metode"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mengambil tipe file yang didukung."
type: docs
url: /id/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

Mengambil tipe file yang didukung.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### Contoh

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Ambil koleksi tipe file yang didukung
    supported_file_types = FileType.get_supported_file_types()

    # Enumerasikan tipe file yang diurutkan berdasarkan ekstensi
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### Lihat Juga
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
