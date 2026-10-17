---
title: "Redaksi metadata"
linkTitle: "Metadata redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menunjukkan bagaimana API redaksi Python memungkinkan Anda mengganti atau menghapus metadata menggunakan filter atau pencarian dengan ekspresi reguler."
type: docs
url: /id/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Dengan API GroupDocs.Redaction Anda dapat menerapkan redaksi metadata untuk dokumen dengan berbagai format seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya. Lihat daftar lengkap pada artikel [supported document formats]().

GroupDocs.Redactions menyediakan API fleksibel yang memungkinkan mengganti atau menghapus metadata menggunakan filter atau pencarian dengan ekspresi reguler.

## Filter metadata

Fungsi dasar untuk semua redaksi, yang diturunkan dari kelas dasar [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) adalah *metadata filtering* dan wajib untuk redaksi metadata. Ini menggunakan enumerasi bertanda [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), yang berisi item untuk entri metadata paling sering. Anda dapat mengatur filter ke *All*, atau kombinasi metadata apa pun. Misalnya, contoh di bawah mengatur filter ke *Author*, *Manager*, dan *NameOfApplication* — untuk redaksi teks atau membersihkannya:

```python
# redaksi yang diturunkan dari MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Berikut adalah tabel dengan daftar lengkap item [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Filter | Nilai numerik | Deskripsi |
| --- | --- | --- |
| *None* | 0 | Pengaturan filter kosong, tidak cocok dengan item metadata apa pun |
| *Author* | 1 | Penulis dokumen |
| *Kategori* | 2 | Kategori dokumen |
| *Komentar* | 4 | Komentar dokumen |
| *Perusahaan* | 8 | Perusahaan Penulis |
| *ContentStatus* | 16 | Status konten |
| *CreatedTime* | 32 | Waktu pembuatan |
| *HyperlinkBase* | 64 | Basis hyperlink |
| *LastPrinted* | 128 | Tanggal dan waktu cetak terakhir |
| *LastSavedBy* | 256 | Terakhir disimpan oleh pengguna |
| *LastSavedTime* | 1024 | Tanggal dan waktu terakhir disimpan |
| *NameOfApplication* | 2048 | Nama aplikasi tempat dokumen dibuat |
| *Manager* | 4096 | Nama manajer penulis |
| *RevisionNumber* | 8192 | Nomor revisi |
| *Subject* | 16384 | Subjek dokumen |
| *Template* | 32768 | Nama templat dokumen |
| *Title* | 65536 | Judul dokumen |
| *TotalEditingTime* | 131072 | Total waktu penyuntingan |
| *Versi* | 262144 | Versi dokumen |
| *Deskripsi* | 524288 | Deskripsi dokumen |
| *Kata Kunci* | 1048576 | Kata kunci dokumen |
| *ContentType* | 2097152 | Tipe konten |
| *Semua* | 2147483647 | Semua jenis item metadata |

## Clean metadata

Anda dapat mengganti semua atau metadata tertentu dalam dokumen dengan nilai kosong (kosong atau minimal) menggunakan kelas [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/). Contoh di bawah ini mengosongkan semua properti dokumen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Tentukan opsi redaksi untuk menghapus semua metadata
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(met_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Anda dapat menentukan [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) atau menggunakan konstruktor default untuk mengosongkan semua metadata dalam dokumen yang diberikan, Custom - untuk menghapus semua entri metadata khusus.

## Redact metadata

Anda dapat menggunakan [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) untuk menghapus data sensitif dari metadata dokumen menggunakan ekspresi reguler. Misalnya, kita dapat menghapus semua penyebutan "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Tentukan opsi redaksi: pola pencarian dan string pengganti
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(met_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Argumen pertama adalah ekspresi reguler, argumen kedua adalah string pengganti. Anda juga dapat menentukan ruang lingkup redaksi dengan mengatur filter, misalnya ke [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - ini akan membiarkan kecocokan ekspresi reguler tidak diubah pada semua item metadata, kecuali properti "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Tentukan opsi redaksi: pola pencarian dan string pengganti
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Batasi ruang lingkup redaksi hanya pada item metadata Company
    met_red.filter = MetadataFilters.COMPANY

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(met_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Semua redaksi metadata diterapkan pada setiap item metadata secara terpisah, dan bahkan jika redaksi pada suatu item metadata gagal, item metadata lainnya akan tetap diperbarui. Anda dapat menemukan daftar item metadata yang gagal, dilewati (ditolak) dan alasannya di properti [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) dari [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
