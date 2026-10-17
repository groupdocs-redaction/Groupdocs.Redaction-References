---
title: "Dapatkan format file yang didukung"
linkTitle: "Get supported file formats"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan cara mendapatkan daftar semua format file yang didukung oleh GroupDocs.Redaction menggunakan Python."
type: docs
url: /id/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction memungkinkan Anda mendapatkan daftar semua format file yang didukung dengan langkah-langkah berikut:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

Contoh berikut menunjukkan cara mendapatkan daftar format file yang didukung.

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

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)
