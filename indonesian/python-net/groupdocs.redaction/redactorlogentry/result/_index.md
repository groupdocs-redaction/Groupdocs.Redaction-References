---
title: "properti result"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Hasil yang dikembalikan oleh DocumentFormatInstance."
type: docs
url: /id/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Hasil yang dikembalikan oleh [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Semua redaksi metadata diterapkan pada setiap item metadata secara terpisah, dan bahkan jika redaksi sebuah item metadata gagal, item metadata lainnya akan diperbarui. Anda dapat menemukan daftar item metadata yang gagal, dilewati (ditolak) dan alasan untuk itu di properti `ErrorMessage` dari [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Lihat Juga
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
