---
title: "Kelas MetadataSearchRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi metadata yang mencari dan menghapus metadata menggunakan ekspresi reguler, mencocokkan kunci dan/atau nilai."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Mewakili redaksi metadata yang mencari dan menghapus metadata menggunakan ekspresi reguler, mencocokkan kunci dan/atau nilai.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Tipe MetadataSearchRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Menginisialisasi instance baru dari kelas MetadataSearchRedaction, menggunakan nilai untuk mencocokkan item yang disensor. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Menginisialisasi instance baru dari MetadataSearchRedaction, menggunakan nama item dan nilai untuk mencocokkan item yang disensor. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Menginisialisasi instance baru dari kelas MetadataSearchRedaction, menggunakan nilai untuk mencocokkan item yang disensor. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Menginisialisasi instance baru dari MetadataSearchRedaction menggunakan nama item dan nilai untuk mencocokkan item yang disensor. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Menerapkan redaksi pada sebuah instance format yang diberikan. (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Deskripsi redaksi, berisi nama dan parameternya. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Ekspresi reguler untuk mencocokkan nama (kunci) dari sebuah item metadata. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Nilai penggantian teks. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Ekspresi reguler untuk mencocokkan teks nilai dari sebuah item metadata. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Filter yang digunakan untuk memilih semua atau metadata tertentu, seperti Author atau Company. (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Sembunyikan setiap nilai metadata yang cocok dengan pola
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Panduan tugas yang menggunakan `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
