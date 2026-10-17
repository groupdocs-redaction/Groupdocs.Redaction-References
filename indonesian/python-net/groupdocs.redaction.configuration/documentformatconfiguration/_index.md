---
title: "Kelas DocumentFormatConfiguration"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili referensi tipe untuk kelas turunan DocumentFormatInstance dan daftar ekstensi file yang didukung untuk deteksi format yang lebih cepat."
type: docs
url: /id/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Mewakili referensi tipe untuk kelas turunan [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) dan daftar ekstensi file yang didukung untuk deteksi format yang lebih cepat.

Pelajari lebih lanjut

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Tipe DocumentFormatConfiguration menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Menginisialisasi sebuah instance baru dari DocumentFormatConfiguration. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Memeriksa apakah ekstensi file yang diberikan dapat ditangani sebagai DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Tipe kelas yang mewarisi dari [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Daftar ekstensi file yang dipisahkan koma (misalnya \".pdf\"), tidak sensitif huruf. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Data yang diperlukan untuk inisialisasi [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Contoh

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Buat konfigurasi format khusus
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Lihat Juga
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
