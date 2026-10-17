---
title: "Kelas ReplacementOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili opsi untuk penggantian teks yang cocok."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Mewakili opsi untuk penggantian teks yang cocok.

Pelajari lebih lanjut

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Tipe ReplacementOptions menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Menginisialisasi instance baru dari ReplacementOptions dengan teks pengganti yang ditentukan. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Menginisialisasi instance baru dari kelas ReplacementOptions dengan persegi panjang berwarna sebagai opsi. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Aksi penggantian: menggambar kotak atau mengganti teks. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Warna untuk opsi `ReplacementType.draw_box` (diabaikan jika tidak). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Penanganan redaksi khusus yang memungkinkan pengguna mendefinisikan logika redaksi mereka sendiri. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Array filter yang akan diterapkan dengan redaksi ini. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Nilai penggantian teks. |

### Contoh

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Ganti teks yang cocok dengan placeholder "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Panduan tugas yang menggunakan `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
