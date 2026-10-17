---
title: "metode load"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Memuat RedactionPolicy dari file XML."
type: docs
url: /id/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Memuat RedactionPolicy dari file XML.

```python
def load(cls, file_path):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_path | `str` | Jalur ke file XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Contoh

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Memuat instance RedactionPolicy dari aliran yang berisi konfigurasi XML.

```python
def load(cls, input):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| input | `io.RawIOBase` | Stream yang berisi konfigurasi XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Contoh

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Muat kebijakan dari file XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Terapkan kebijakan ke dokumen
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Lihat Juga
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
