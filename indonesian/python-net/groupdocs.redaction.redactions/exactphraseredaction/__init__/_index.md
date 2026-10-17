---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru ExactPhraseRedaction dalam mode tidak sensitif huruf."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Menginisialisasi instance baru ExactPhraseRedaction dalam mode tidak sensitif huruf.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| search_phrase | `str` | String untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |

### Contoh

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Ganti kemunculan "John Doe" dengan "[CUSTOMER]" (tidak peka huruf)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Menginisialisasi instance ExactPhraseRedaction baru.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| search_phrase | `str` | String untuk mencari dan mengganti. |
| is_case_sensitive | `bool` | True jika pencarian peka huruf diperlukan. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |

### Contoh

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Redaksi frasa tepat tidak peka huruf
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Redaksi frasa tepat peka huruf
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Lihat Juga
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
