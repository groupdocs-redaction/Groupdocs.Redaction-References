---
title: "Hapus redaksi halaman"
linkTitle: "Remove page redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan cara menghapus halaman yang berisi data sensitif dari dokumen PDF, presentasi, dan spreadsheet Anda."
type: docs
url: /id/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction memungkinkan dengan mudah menghapus halaman dari dokumen PDF, slide dari presentasi, dan lembar kerja dari dokumen spreadsheet.

Dengan API GroupDocs.Redaction Anda dapat menghapus halaman dengan menentukan rentang halaman berdasarkan posisi relatifnya (awal atau akhir), indeks berbasis nol, dan jumlah halaman yang akan dihapus. Saat ini format yang didukung meliputi: PDF, presentasi (Microsoft PowerPoint, OpenOffice Presentations), dokumen pengolah kata (Microsoft Word, OpenOffice Texts, Rich Text Files), spreadsheet (Microsoft Excel, OpenOffice Spreadsheets, dll.) dan gambar multi-frame.

## Remove page range

Pada contoh di bawah, kami menghapus halaman ke-2, ke-3, dan ke-4 dari dokumen, jika dokumen memiliki cukup halaman:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Muat dokumen yang akan direduksi
    with Redactor("./multipage_sample.pdf") as redactor:
        # Dapatkan info dokumen
        doc_info = redactor.get_document_info()

        # Membutuhkan setidaknya 4 halaman
        if doc_info.page_count > 3:
            # Hapus 3 halaman mulai dari halaman ke-2 (indeks berbasis nol 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Terapkan penyensoran
            result = redactor.apply(rem_opt)

            # Simpan dokumen yang telah diredaksi di samping file sumber
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) untuk mengunduhnya.

## Remove last page

Dalam beberapa kasus Anda mungkin perlu menghapus halaman terakhir atau sejumlah halaman, terlepas dari berapa banyak halaman yang ada.

Contoh berikut menunjukkan cara menghapus halaman terakhir dari sebuah dokumen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Hapus 1 halaman menghitung dari akhir dokumen
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Muat dokumen yang akan direduksi
    with Redactor("./multipage_sample.pdf") as redactor:
        # Dapatkan info dokumen
        doc_info = redactor.get_document_info()

        # Membutuhkan setidaknya 2 halaman agar dokumen tidak menjadi kosong
        if doc_info.page_count > 1:
            # Terapkan penyensoran
            result = redactor.apply(rem_opt)

            # Simpan dokumen yang telah diredaksi di samping file sumber
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) untuk mengunduhnya.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Jika berupa gambar multi-frame, Anda mungkin perlu menghapus sejumlah frame (diperlakukan sebagai "halaman").

Contoh berikut menunjukkan cara menghapus 3 frame dari gambar GIF animasi:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Hapus frame mulai dari yang ke-3 (indeks berbasis nol 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Muat gambar multi-frame yang akan diredaksi
    with Redactor("./sample.gif") as redactor:
        # Dapatkan info dokumen
        doc_info = redactor.get_document_info()

        # Membutuhkan setidaknya 7 frame
        if doc_info.page_count >= 7:
            # Terapkan penyensoran
            result = redactor.apply(rem_opt)

            # Simpan gambar yang diredaksi di samping file sumber
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) untuk mengunduhnya.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
