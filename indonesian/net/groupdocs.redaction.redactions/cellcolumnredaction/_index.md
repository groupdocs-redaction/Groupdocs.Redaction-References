---
title: CellColumnRedaction
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Merupakan redaksi teks yang menggantikan teks dalam dokumen spreadsheet CSV Excel dll..
type: docs
weight: 450
url: /id/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Merupakan redaksi teks yang menggantikan teks dalam dokumen spreadsheet (CSV, Excel, dll.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Menginisialisasi instance baru dari kelas CellColumnRedaction. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Mendapatkan[`ReplacementOptions`](../replacementoptions) misalnya, menentukan jenis penggantian teks. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Mengembalikan sebuah string, menjelaskan redaksi dan parameternya. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Mendapat filter kolom dan lembar kerja. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Mendapat atau menyetel[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementasi, diperlukan untuk mengekstrak teks dari konten grafik. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Mencocokkan ekspresi reguler. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Menerapkan redaksi ke instance format tertentu. |

### Perkataan

**Belajarlah lagi**

* Detail lebih lanjut tentang menerapkan redaksi: [Dasar redaksi](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Detail lebih lanjut tentang penyuntingan spreadsheet: [Redaksi spreadsheet](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Contoh

Contoh berikut menunjukkan penghapusan email pengguna dari kolom kedua pada lembar kerja "Pelanggan" dari dokumen spreadsheet.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // kolom ke-2 berbasis nol
       WorkSheetName = "Customers"
   };
   var expression = new Regex("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
   RedactorChangeLog changeLog = redactor.Apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
   if (result.Status != RedactionStatus.Failed)
   {
      doc.Save(new SaveOptions() { AddSuffix = true });
   };
}
```

### Lihat juga

* class [TextRedaction](../textredaction)
* ruang nama [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
