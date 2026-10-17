---
title: "metode remove_pages"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menghapus satu atau beberapa halaman tergantung pada posisi awal, offset, dan jumlahnya."
type: docs
url: /id/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Menghapus satu atau beberapa halaman tergantung pada posisi awal, offset, dan jumlahnya.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Posisi asal pencarian, awal atau akhir dokumen. |
| index | `int` | Indeks posisi mulai (berbasis 0). |
| count | `int` | Jumlah halaman yang akan dihapus. |

**Returns:** Pages removal redaction result.

### Lihat Juga
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
