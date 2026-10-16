---
title: "com.groupdocs.redaction.redactions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Paket ini menyediakan kelas untuk berbagai jenis penyuntingan."
type: docs
weight: 16
url: /id/java/com.groupdocs.redaction.redactions/
---

Paket ini menyediakan kelas untuk berbagai jenis penyuntingan.



## Kelas

| Kelas | Deskripsi |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Mewakili redaksi yang mengganti teks anotasi (komentar, dll.) yang cocok dengan ekspresi reguler tertentu. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Mewakili redaksi teks yang mengganti teks dalam dokumen spreadsheet (CSV, Excel, dll.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Menyediakan opsi untuk membatasi cakupan CellColumnRedaction ke lembar kerja dan kolom. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Menyediakan data masukan untuk [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Mewakili hasil yang dikembalikan oleh [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Mewakili redaksi teks yang menghapus anotasi jika teks cocok dengan ekspresi reguler yang diberikan (secara opsional menghapus semua anotasi). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Mewakili redaksi metadata yang menghapus semua metadata atau metadata yang cocok dengan MetadataFilters tertentu dari dokumen. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Mewakili redaksi teks yang mengganti frasa tepat dalam teks dokumen, tidak sensitif huruf besar/kecil secara default. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Mewakili redaksi yang menempatkan persegi panjang berwarna di area tertentu dari dokumen gambar. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Mewakili daftar tipe metadata dokumen yang paling umum. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Mewakili kelas abstrak dasar untuk redaksi metadata dokumen. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Mewakili redaksi metadata yang mencari dan menghapus metadata menggunakan ekspresi reguler, mencocokkan kunci dan/atau nilai. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Mewakili filter redaksi, mengatur area dalam sebuah halaman dokumen untuk menerapkan redaksi. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Mewakili redaksi tekstual kompleks yang memengaruhi teks, gambar, dan anotasi dalam area halaman. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Mewakili filter redaksi, mengatur rentang halaman dalam dokumen untuk menerapkan redaksi. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Mewakili informasi aksi perubahan tunggal yang dilakukan selama proses redaksi. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Mewakili filter redaksi, mengatur ruang lingkup dalam dokumen untuk menerapkan redaksi. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Mewakili jenis data dokumen yang terpengaruh oleh redaksi. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Mewakili redaksi teks yang mencari dan mengganti teks dalam dokumen dengan mencocokkan ekspresi reguler yang diberikan. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Mewakili parameter warna dan area untuk penggantian wilayah gambar. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Mewakili redaksi yang menghapus sebuah halaman (slide, lembar kerja, dll.) dari dokumen. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Mewakili opsi untuk penggantian teks yang cocok. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Mewakili kelas abstrak dasar untuk redaksi teks dokumen. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Mewakili informasi penggantian tekstual. |

## Antarmuka

| Antarmuka | Deskripsi |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Mendefinisikan callback redaksi khusus. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Mendefinisikan metode yang diperlukan untuk menerima informasi tentang setiap perubahan redaksi dan secara opsional mencegahnya. |

## Enumerasi

| Enum | Deskripsi |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Menyediakan bidang yang mewakili titik referensi dalam dokumen untuk pencarian. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Mewakili tindakan yang dapat diambil untuk melakukan redaksi. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Mewakili jenis penggantian untuk teks yang cocok. |
