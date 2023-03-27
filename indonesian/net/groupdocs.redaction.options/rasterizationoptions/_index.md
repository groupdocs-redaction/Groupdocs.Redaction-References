---
title: RasterizationOptions
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Menyediakan opsi untuk mengubah file menjadi PDF.
type: docs
weight: 350
url: /id/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Menyediakan opsi untuk mengubah file menjadi PDF.

```csharp
public class RasterizationOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Menginisialisasi instance baru. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Mendapatkan atau menyetel tingkat Kepatuhan PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah semua halaman dalam dokumen perlu diubah menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, atur ke FALSE untuk menghindari rasterisasi. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Mendapat indikator, yang bernilai benar jika opsi rasterisasi lanjutan disetel. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Mendapat atau mengatur jumlah halaman yang akan diubah menjadi PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Mendapat atau mengatur indeks halaman pertama (berbasis 0) untuk diubah menjadi PDF. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan untuk diterapkan. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan untuk diterapkan. |

### Perkataan

**Belajarlah lagi**

* Detail lebih lanjut tentang menyimpan dokumen sebagai PDF raster: [Simpan dalam PDF raster](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Detail lebih lanjut tentang opsi rasterisasi: [Pilih halaman tertentu untuk PDF raster](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Contoh

Contoh berikut menunjukkan cara menyetel opsi untuk proses rasterisasi.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // menyunting data sensitif pada slide pertama 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi lanjutan dengan pengaturan default.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan opsi default (konversi halaman menjadi gambar, simpan sebagai PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi tingkat lanjut perbatasan dengan pengaturan khusus.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan batas khusus
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi tingkat lanjut derau dengan pengaturan khusus.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan nomor kustom dan ukuran efek derau
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Contoh berikut menunjukkan cara menerapkan opsi tilt advanced rasterization dengan pengaturan kustom.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan efek kemiringan khusus
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Lihat juga

* ruang nama [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
