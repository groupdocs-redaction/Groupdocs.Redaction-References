---
title: "metode find_format"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menemukan konfigurasi format untuk ekstensi file tertentu."
type: docs
url: /id/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Menemukan konfigurasi format untuk ekstensi file tertentu.

```python
def find_format(self, file_extension):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_extension | `str` | Ekstensi file, formatnya adalah ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Contoh

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Dapatkan instance konfigurasi singleton
config = RedactorConfiguration.get_instance()

# Ambil pengaturan format untuk ekstensi tertentu
settings = config.find_format(".txt")
if settings:
    # Perluas daftar ekstensi yang ditangani, mis., tambahkan .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Lihat Juga
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
