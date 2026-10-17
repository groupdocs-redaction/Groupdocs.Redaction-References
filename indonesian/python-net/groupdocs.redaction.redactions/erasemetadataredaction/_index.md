---
title: "Kelas EraseMetadataRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi metadata yang menghapus semua metadata atau metadata yang cocok dengan MetadataFilters tertentu dari dokumen."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Mewakili redaksi metadata yang menghapus semua metadata atau metadata yang cocok dengan MetadataFilters tertentu dari dokumen.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Tipe EraseMetadataRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Menginisialisasi instance baru kelas EraseMetadataRedaction, menghapus semua metadata. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Menginisialisasi sebuah instance baru dari EraseMetadataRedaction, menghapus metadata yang cocok dengan `MetadataFilters` yang ditentukan. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Menerapkan redaksi pada sebuah instance format yang diberikan. (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Deskripsi redaksi dan parameternya. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Filter yang digunakan untuk memilih semua atau metadata tertentu, seperti Author atau Company. (diturunkan dari [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Hapus semua metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Hapus hanya bidang author
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Panduan tugas yang menggunakan `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
