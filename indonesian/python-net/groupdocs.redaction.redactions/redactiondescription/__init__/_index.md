---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi sebuah instance baru dari kelas RedactionDescription tanpa informasi penggantian."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Menginisialisasi sebuah instance baru dari kelas RedactionDescription tanpa informasi penggantian.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redaction_type | `RedactionType` | Jenis data yang disensor. |
| action_type | `RedactionActionType` | Tindakan yang akan dilakukan pada data ini. |
| original_text | `str` | Teks yang cocok, komentar, atau isi anotasi. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Menginisialisasi sebuah instance baru dari kelas RedactionDescription dengan informasi penggantian.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redaction_type | `RedactionType` | Jenis data yang disensor. |
| action_type | `RedactionActionType` | Tindakan yang akan dilakukan pada data ini. |
| original_text | `str` | Teks yang cocok, komentar, atau isi anotasi. |
| replacement | `TextReplacement` | Teks pengganti, teks yang cocok, dan posisinya dalam string asli. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Menginisialisasi RedactionDescription baru dengan informasi penggantian area gambar.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redaction_type | `RedactionType` | Jenis data yang disensor. |
| action_type | `RedactionActionType` | Tindakan yang akan dilakukan pada data ini. |
| image_area_replacement | `RegionReplacementOptions` | Informasi penggantian area gambar. |
| image_details | `str` | Deskripsi teks gambar, secara default adalah string kosong. |

### Lihat Juga
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
