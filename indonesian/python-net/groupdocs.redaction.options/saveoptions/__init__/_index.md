---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance baru dengan pengaturan default: rasterizetopdf bernilai False dan addsuffix bernilai False."
type: docs
url: /id/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi instance baru dengan pengaturan default: rasterize_to_pdf adalah False dan add_suffix adalah False.

```python
def __init__(self):
    ...
```

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Menginisialisasi instance baru dengan parameter yang diberikan.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, jika semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. |
| suffix | `str` | Teks ini akan ditambahkan ke akhir nama file; jika tidak kosong juga akan mengatur `add_suffix` menjadi True. |

### Contoh

```python
from groupdocs.redaction.options import SaveOptions

# Buat opsi penyimpanan dengan pengaturan default
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Lihat Juga
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
