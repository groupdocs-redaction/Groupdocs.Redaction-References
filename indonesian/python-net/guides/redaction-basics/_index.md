---
title: "Dasar-dasar redaksi"
linkTitle: "Redaction basics"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan cara pengembang Python dapat menerapkan redaksi metadata, gambar, anotasi, dan teks dalam dokumen mereka. Berbagai format dokumen didukung, seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya."
type: docs
url: /id/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction mendukung serangkaian fitur redaksi dokumen yang efektif. Ini memungkinkan penerapan redaksi untuk [teks](), [metadata](), [anotasi](), [gambar]().

Berbagai format dokumen didukung, seperti: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya. Lihat daftar lengkap format yang didukung pada artikel [format dokumen yang didukung]().

## Redaction types

GroupDocs.Redaction dilengkapi dengan tipe redaksi berikut:

| Tipe | Deskripsi | Kelas |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Menerapkan redaksi pada dokumen dilakukan melalui metode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . Sebagai hasilnya, Anda menerima instance [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) , yang berisi entri log untuk setiap redaksi yang diterapkan. Entri tersebut berisi referensi ke instance [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) termasuk opsi‑opsinya, status operasi (lihat di bawah) dan deskripsi teks bila berlaku. Jika setidaknya satu redaksi gagal, Anda akan melihat [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) :

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Simpan dokumen yang telah diredaksi di samping file sumber
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Semua status yang mungkin dari enumerasi [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) tercantum dalam tabel ini:

| Status | Deskripsi | Alasan yang mungkin |
| --- | --- | --- |
| *Applied* | Redaksi diterapkan sepenuhnya dan berhasil | Semua operasi dalam proses redaksi berhasil diterapkan |
| *PartiallyApplied* | Redaksi diterapkan hanya pada sebagian dari kecocokannya | 1) Batas percobaan untuk penggantian terlampaui2) Setidaknya satu perubahan ditolak oleh pengguna |
| *Skipped* | Redaksi dilewati (tidak diterapkan) | 1) Batas percobaan untuk redaksi terlampaui2) Redaksi tidak dapat diterapkan pada jenis dokumen ini3) Semua penggantian ditolak oleh pengguna dan tidak ada perubahan yang dibuat |
| *Failed* | Redaksi gagal dengan pengecualian | Terjadi pengecualian dalam proses redaksi |

Untuk informasi terperinci, Anda harus mengiterasi entri log redaksi di [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) dan memeriksa properti [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) pada setiap item dengan status selain *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Secara default, dokumen yang telah direduksi disimpan dalam format PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Ekspor semua redaksi yang gagal atau dilewati
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Anda dapat menerapkan sebanyak mungkin redaksi yang Anda perlukan dalam satu panggilan ke metode [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , karena overload‑nya menerima array redaksi dan kebijakan redaksi. Dalam kasus ini, redaksi akan diterapkan dalam urutan yang sama seperti muncul dalam array. Sebagai alternatif untuk menentukan set redaksi dalam kode Anda, Anda dapat membuat file XML dengan kebijakan redaksi, seperti yang dijelaskan [here]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Berikan daftar redaksi yang akan diterapkan secara berurutan
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan daftar redaksi
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Secara default, dokumen yang telah direduksi disimpan dalam format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Ekspor semua redaksi yang gagal atau dilewati
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) untuk mengunduhnya.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
