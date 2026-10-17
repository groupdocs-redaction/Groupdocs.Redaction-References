---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru kelas EraseMetadataRedaction, menghapus semua metadata."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi instance baru kelas EraseMetadataRedaction, menghapus semua metadata.

```python
def __init__(self):
    ...
```

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

Menginisialisasi sebuah instance baru dari EraseMetadataRedaction, menghapus metadata yang cocok dengan `MetadataFilters` yang ditentukan.

```python
def __init__(self, filter):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| filter | `MetadataFilters` | Filter untuk metadata yang akan dihapus. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Hapus semua metadata
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Hapus hanya bidang metadata penulis
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Lihat Juga
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
