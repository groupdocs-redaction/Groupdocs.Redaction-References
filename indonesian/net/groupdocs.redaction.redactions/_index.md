---
title: GroupDocs.Redaction.Redactions
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: ItuRedactions namespace menyediakan kelas untuk berbagai jenis redaksi.
type: docs
weight: 70
url: /id/net/groupdocs.redaction.redactions/
---
ItuRedactions namespace menyediakan kelas untuk berbagai jenis redaksi.

## Kelas

| Kelas | Keterangan |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Merupakan redaksi yang menggantikan teks anotasi (komentar, dll.) yang cocok dengan ekspresi reguler yang diberikan. |
| [CellColumnRedaction](./cellcolumnredaction) | Merupakan redaksi teks yang menggantikan teks dalam dokumen spreadsheet (CSV, Excel, dll.). |
| [CellFilter](./cellfilter) | Memberikan opsi untuk membatasi ruang lingkup a[`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) ke lembar kerja dan kolom. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Merupakan redaksi teks yang menghapus anotasi jika teks cocok dengan ekspresi reguler yang diberikan (opsional menghapus semua anotasi). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Merupakan redaksi metadata yang menghapus semua metadata atau metadata yang cocok dengan MetadataFilters tertentu dari dokumen. |
| [ExactPhraseRedaction](./exactphraseredaction) | Mewakili redaksi teks yang menggantikan frase persis dalam teks dokumen, secara default tidak peka huruf besar/kecil. |
| [ImageAreaRedaction](./imagearearedaction) | Merupakan redaksi yang menempatkan persegi panjang berwarna di area tertentu dari dokumen gambar. |
| [MetadataRedaction](./metadataredaction) | Merupakan kelas abstrak dasar untuk redaksi metadata dokumen. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Mewakili redaksi metadata yang mencari dan menyunting metadata menggunakan ekspresi reguler, kunci dan/atau nilai yang cocok. |
| [RedactionDescription](./redactiondescription) | Merupakan info tindakan perubahan tunggal yang dilakukan selama proses redaksi. |
| [RegexRedaction](./regexredaction) | Merupakan redaksi teks yang mencari dan mengganti teks dalam dokumen dengan mencocokkan ekspresi reguler yang diberikan. |
| [RegionReplacementOptions](./regionreplacementoptions) | Mewakili parameter warna dan area untuk penggantian wilayah gambar. Melihat[`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction) . |
| [RemovePageRedaction](./removepageredaction) | Merupakan redaksi yang menghapus halaman (slide, lembar kerja, dll.) dari dokumen. |
| [ReplacementOptions](./replacementoptions) | Merupakan opsi untuk penggantian teks yang cocok. |
| [TextRedaction](./textredaction) | Mewakili kelas abstrak dasar untuk penyuntingan teks dokumen. |
| [TextReplacement](./textreplacement) | Merupakan informasi pengganti tekstual. |
## Antarmuka

| Antarmuka | Keterangan |
| --- | --- |
| [IRedactionCallback](./iredactioncallback) | Menentukan metode yang diperlukan untuk menerima informasi pada setiap perubahan redaksi dan secara opsional mencegahnya. |
## Pencacahan

| Pencacahan | Keterangan |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Menampilkan daftar jenis metadata dokumen yang paling umum. |
| [PageSeekOrigin](./pageseekorigin) | Menyediakan bidang yang mewakili titik referensi dalam dokumen untuk dicari. |
| [RedactionActionType](./redactionactiontype) | Mewakili tindakan yang dapat diambil untuk melakukan redaksi. |
| [RedactionType](./redactiontype) | Mewakili jenis data dokumen, dipengaruhi oleh redaksi. |
| [ReplacementType](./replacementtype) | Merupakan jenis pengganti teks yang cocok. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->