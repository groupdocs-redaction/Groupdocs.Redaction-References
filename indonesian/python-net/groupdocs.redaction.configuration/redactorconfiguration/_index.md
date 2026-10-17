---
title: "Kelas RedactorConfiguration"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyediakan akses ke daftar format yang didukung, format bawaan dan format pengguna khusus."
type: docs
url: /id/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Menyediakan akses ke daftar format yang didukung, format bawaan dan format pengguna khusus.

Pelajari lebih lanjut:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Tipe RedactorConfiguration menampilkan anggota-anggota berikut:

### Metode
| Metode | Deskripsi |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Menemukan konfigurasi format untuk ekstensi file tertentu. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Mengembalikan sebuah instance singleton dengan konfigurasi default dari format bawaan. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Daftar format yang dikenali, lihat [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Contoh

```python
# Tambahkan penangan format pengguna khusus
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Ambil penangan format pengguna bawaan atau khusus
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Lihat Juga
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
