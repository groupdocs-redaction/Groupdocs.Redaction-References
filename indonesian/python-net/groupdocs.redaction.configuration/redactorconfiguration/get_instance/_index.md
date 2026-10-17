---
title: "metode get_instance"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mengembalikan sebuah instance singleton dengan konfigurasi default dari format bawaan."
type: docs
url: /id/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Mengembalikan sebuah instance singleton dengan konfigurasi default dari format bawaan.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Contoh

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Dapatkan konfigurasi singleton
config = RedactorConfiguration.get_instance()

# Perluas ekstensi yang didukung untuk format teks biasa
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Lihat Juga
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
