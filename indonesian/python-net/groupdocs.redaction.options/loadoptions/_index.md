---
title: "Kelas LoadOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyediakan opsi yang akan digunakan untuk membuka file."
type: docs
url: /id/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Menyediakan opsi yang akan digunakan untuk membuka file.

Pelajari lebih lanjut
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Tipe LoadOptions menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Menginisialisasi sebuah instance baru dari kelas LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Menginisialisasi sebuah instance baru dari LoadOptions dengan kata sandi yang ditentukan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Menginisialisasi sebuah instance LoadOptions baru dengan flag pra‑rasterisasi yang ditentukan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Menginisialisasi sebuah instance LoadOptions baru dengan kata sandi yang ditentukan. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Kata sandi untuk dokumen yang dilindungi kata sandi. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Flag pre_rasterize yang menunjukkan apakah berkas harus dipra‑rasterisasi. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Tentukan opsi pemuatan dengan kata sandi dokumen
load_opt = LoadOptions("mypassword")

# Tentukan redaksi
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Buka dokumen yang dilindungi kata sandi
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Simpan dokumen yang telah di‑redact
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Lihat Juga
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
