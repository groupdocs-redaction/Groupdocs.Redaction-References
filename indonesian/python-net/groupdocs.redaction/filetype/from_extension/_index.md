---
title: "metode from_extension"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Memetakan ekstensi file ke tipe file."
type: docs
url: /id/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Memetakan ekstensi file ke tipe file.

```python
def from_extension(cls, extension):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| extension | `str` | Ekstensi file (termasuk titik "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Menaikkan | Deskripsi |
| :- | :- |
| `ValueError` | Ketika `extension` bernilai null atau string kosong. |

### Lihat Juga
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
