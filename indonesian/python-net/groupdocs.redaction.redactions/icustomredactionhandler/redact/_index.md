---
title: "metode redact"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menerapkan penyensoran khusus pada konten dokumen tertentu."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Menerapkan penyensoran khusus pada konten dokumen tertentu.

Saat ini, ini hanya didukung untuk PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Pengguna dapat mendefinisikan logika redaksi mereka sendiri, seperti redaksi berbasis AI, yang mungkin lebih maju daripada metode berbasis pola sederhana.

```python
def redact(self, context):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| context | `CustomRedactionContext` | Berisi konten dokumen yang akan disensor beserta metadata terkait. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Lihat Juga
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
