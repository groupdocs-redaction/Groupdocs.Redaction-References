---
title: "Redaksi anotasi"
linkTitle: "Annotation redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan implementasi redaksi anotasi untuk dokumen dengan berbagai format seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya."
type: docs
url: /id/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Dengan API GroupDocs.Redaction Anda dapat menerapkan redaksi anotasi untuk dokumen dengan berbagai format seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya. Lihat daftar lengkap pada artikel [format dokumen yang didukung]().

GroupDocs.Redactions menyediakan API fleksibel yang memungkinkan menghapus data sensitif dari teks anotasi, atau menghapus anotasi sepenuhnya menggunakan ekspresi reguler.

## Remove annotations (comments etc)

Anda dapat menggunakan GroupDocs.Redaction untuk menghapus semua atau komentar tertentu serta anotasi lain dari dokumen. Misalnya, kita dapat menghapus semua komentar dari dokumen yang berisi teks seperti "use", "show", atau "describe" dalam isinya:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Tentukan opsi redaction untuk menghapus anotasi yang cocok dengan pola
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Muat dokumen yang akan direduksi
    with Redactor("./annotated.xlsx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(a_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) untuk mengunduhnya.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Anda dapat menggunakan konstruktor tanpa argumen untuk menghapus semua anotasi dalam dokumen.

## Redact annotations

Alih-alih menghapus semua atau anotasi tertentu, Anda dapat menghapus data sensitif dari teks anotasi. Misalnya, kita dapat menghapus semua penyebutan "John" dalam dokumen yang diberikan, misalnya:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Tentukan opsi redaksi: pola pencarian dan string pengganti
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Muat dokumen yang akan direduksi
    with Redactor("./annotated.xlsx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(a_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) untuk mengunduhnya.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
