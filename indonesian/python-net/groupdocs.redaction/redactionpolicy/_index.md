---
title: "Kelas RedactionPolicy"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili kebijakan sanitasi, berisi sekumpulan redaksi spesifik yang akan diterapkan."
type: docs
url: /id/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Mewakili kebijakan sanitasi, berisi sekumpulan redaksi spesifik yang akan diterapkan.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Tipe RedactionPolicy menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Menginisialisasi instance RedactionPolicy baru. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Menginisialisasi RedactionPolicy baru dengan daftar redaksi tertentu. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Memuat RedactionPolicy dari file XML. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Memuat instance RedactionPolicy dari aliran yang berisi konfigurasi XML. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Menyimpan kebijakan redaksi ke file. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Menyimpan kebijakan redaksi ke aliran. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Daftar kelas turunan [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/) yang sepenuhnya dikonfigurasi. |

### Contoh

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Bangun kebijakan yang dapat digunakan kembali di memori
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Terapkan kebijakan ke dokumen
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Panduan tugas yang menggunakan `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Lihat Juga
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
