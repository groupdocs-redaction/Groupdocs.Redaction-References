---
title: "Halo, Dunia!"
linkTitle: "Hello, World!"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mulai dengan cepat menggunakan GroupDocs.Redaction untuk Python via .NET dengan membuat dan menjalankan contoh sederhana."
type: docs
url: /id/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Contoh "Hello, World!" sering menjadi langkah pertama saat menjelajahi GroupDocs.Redaction untuk Python via .NET. Ini berfungsi sebagai tes sederhana untuk memastikan bahwa lingkungan pengembangan Anda telah disiapkan dengan benar dan bahwa perpustakaan berfungsi seperti yang diharapkan.

## Overview
GroupDocs.Redaction untuk Python via .NET memungkinkan Anda mencari, men-redact, dan menghapus informasi sensitif dari berbagai format dokumen. Berbagai [format yang didukung](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) membuatnya fleksibel untuk berbagai kasus penggunaan.

## How to redact a document
Langkah-langkah berikut menunjukkan cara men-redact informasi sensitif dari sebuah dokumen menggunakan GroupDocs.Redaction untuk Python via .NET:

1. Impor kelas `groupdocs.redaction` yang Anda perlukan.
2. Jelaskan redaction (di sini, frasa tepat yang akan diganti dengan kotak berwarna).
3. Buat instance sebuah [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) dengan jalur ke dokumen contoh.
4. Terapkan redaction.
5. Simpan hasilnya.

## Complete example
Contoh di bawah menggantikan setiap kemunculan frasa "John Doe" dengan kotak merah semi-transparan dan menyimpan dokumen yang telah di-redact:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Gambar kotak merah semi-transparan di atas setiap kemunculan "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Muat dokumen, terapkan redaction, dan simpan hasilnya
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) untuk mengunduhnya.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Contoh ini meraster hasil menjadi PDF bernama `sample_redacted.pdf`, sehingga konten yang di-redact tidak dapat dipulihkan (`save()` meraster ke PDF secara default; opsi `redacted_file_suffix` hanya mengontrol nama output). Untuk mempertahankan format asli, atur `rasterize_to_pdf = False`.

## Additional resources
Demo ini merujuk pada [contoh kode](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) GroupDocs.Redaction untuk Python via .NET.
