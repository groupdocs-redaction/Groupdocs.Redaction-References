---
title: GroupDocs.Redaction.Integration
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: ItuIntegrationnamespace menyediakan antarmuka dan kelas digunakan untuk mengintegrasikan dokumen dengan format berbeda dengan GroupDocs.Redaction.
type: docs
weight: 40
url: /id/net/groupdocs.redaction.integration/
---
ItuIntegrationnamespace menyediakan antarmuka dan kelas, digunakan untuk mengintegrasikan dokumen dengan format berbeda dengan GroupDocs.Redaction.

## Kelas

| Kelas | Keterangan |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Merupakan format tertentu dari sebuah dokumen. Terapkan kelas ini untuk menambahkan jenis dokumen Anda sendiri. |
| [MetadataCollection](./metadatacollection) | Mewakili kamus[`MetadataItem`](../groupdocs.redaction.integration/metadataitem) dengan judulnya sebagai kunci. |
| [MetadataItem](./metadataitem) | Mewakili item metadata, umum untuk semua format yang didukung dan digunakan dalam redaksi metadata. |
## Antarmuka

| Antarmuka | Keterangan |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Menentukan metode yang diperlukan untuk mengakses anotasi, seperti komentar. Perlu dilaksanakan oleh[`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) -derived class untuk melakukan redaksi anotasi. |
| [ICellularFormatInstance](./icellularformatinstance) | Menentukan metode yang diperlukan untuk mengakses format spreadsheet, memiliki satu atau banyak lembar kerja. |
| [IImageFormatInstance](./iimageformatinstance) | Menentukan metode yang diperlukan untuk redaksi format gambar raster. |
| [IMetadataAccess](./imetadataaccess) | Menentukan metode yang diperlukan untuk mengakses metadata dokumen, jika format mendukungnya. |
| [IPaginatedDocument](./ipaginateddocument) | Menentukan metode yang diperlukan untuk memanipulasi halaman dokumen. Perlu dilaksanakan oleh[`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) -derived class untuk melakukan redaksi halaman. |
| [IPreviewable](./ipreviewable) | Menentukan metode untuk membuat pratinjau dokumen. |
| [IRasterizableDocument](./irasterizabledocument) | Menentukan metode yang diperlukan untuk menyimpan dokumen dalam bentuk biner apa pun. Jenis bawaan menyimpan dokumen sebagai PDF dengan gambar halamannya. |
| [ITextualFormatInstance](./itextualformatinstance) | Menentukan metode yang diperlukan untuk menyunting data tekstual dalam dokumen apa pun, yang berisi teks. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
