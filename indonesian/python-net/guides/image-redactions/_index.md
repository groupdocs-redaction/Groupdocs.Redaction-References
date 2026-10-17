---
title: "Redaksi gambar"
linkTitle: "Image redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan cara meredaksi data bersifat sensitif dari gambar dengan berbagai format seperti JPG, PNG, TIFF, dan lainnya."
type: docs
url: /id/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions menyediakan serangkaian fitur untuk meredaksi data bersifat sensitif dari gambar dengan berbagai format seperti JPG, PNG, TIFF, dan lainnya. Lihat daftar lengkapnya di artikel [supported document formats]().

GroupDocs.Redaction mendukung dua cara meredaksi gambar, baik dalam file gambar terpisah maupun gambar yang disematkan:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction untuk Python via .NET juga memungkinkan Anda mengubah metadata gambar (misalnya mengedit data EXIF sebuah gambar atau berfungsi sebagai "penghapus EXIF").

## Redact image area

Untuk meredaksi area gambar, Anda harus menggunakan kelas [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Tentukan posisi kiri-atas dari area yang akan diredaksi
    sample_point = Point(385, 485)
    # Tentukan ukuran area yang perlu diredaksi
    sample_size = Size(1793, 2069)
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Tentukan opsi redaksi
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.jpg") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Secara default, dokumen yang telah direduksi disimpan dalam format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) untuk mengunduhnya.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Jika redaksi tidak dapat diterapkan pada jenis file ini, misalnya dokumen MS Word tanpa gambar yang disematkan, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) akan menjadi [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

Contoh berikut menunjukkan cara mengedit data exif (menghapusnya) dari foto atau gambar lainnya:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Tentukan opsi redaksi untuk menghapus semua metadata gambar (misalnya EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Muat gambar yang akan diredaksi
    with Redactor("./sample.jpg") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(er_opt)

        # Simpan gambar yang diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) untuk mengunduhnya.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Jika redaksi tidak dapat diterapkan pada jenis file ini, misalnya gambar BMP, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) akan menjadi [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Anda dapat meredaksi area gambar dalam semua jenis gambar yang disematkan di dalam dokumen.

Contoh berikut menunjukkan cara meredaksi semua gambar yang disematkan dalam dokumen Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Tentukan posisi kiri-atas dari area yang akan diredaksi
    sample_point = Point(516, 311)
    # Tentukan ukuran area yang perlu diredaksi
    sample_size = Size(170, 35)
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Tentukan opsi redaksi
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan redaksi pada semua gambar yang disematkan
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Secara default, dokumen yang telah direduksi disimpan dalam format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Jika redaksi tidak dapat diterapkan pada jenis file ini, misalnya dokumen spreadsheet, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) akan menjadi [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Anda dapat menghapus frame dari gambar multi-frame dengan asal dan jumlah frame yang diberikan. Untuk informasi tambahan, lihat artikel [remove page redactions]().

Beberapa format gambar, seperti dokumen DjVu, memerlukan [pre-rasterization]() dan penyimpanan lebih lanjut dalam format PDF.
