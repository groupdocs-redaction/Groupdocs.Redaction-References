---
title: "Kelas DeleteAnnotationRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili redaksi teks yang menghapus anotasi jika teks cocok dengan ekspresi reguler tertentu (secara opsional menghapus semua anotasi)."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Mewakili redaksi teks yang menghapus anotasi jika teks cocok dengan ekspresi reguler tertentu (secara opsional menghapus semua anotasi).

Pelajari lebih lanjut

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Tipe DeleteAnnotationRedaction menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, dengan pengaturan untuk menghapus semua anotasi (mencocokkan semua). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, menghapus anotasi yang cocok dengan ekspresi yang diberikan. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Menginisialisasi sebuah instance baru dari kelas DeleteAnnotationRedaction, menghapus anotasi yang cocok dengan ekspresi yang diberikan. |

### Metode
| Metode | Deskripsi |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Menerapkan redaksi pada instance format yang diberikan. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | Deskripsi penyensoran, berisi nama penyensoran dan parameter. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | Ekspresi reguler untuk mencocokkan. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Hapus anotasi yang berisi kata "internal" (tidak peka huruf).
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Panduan tugas yang menggunakan `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Lihat Juga
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
