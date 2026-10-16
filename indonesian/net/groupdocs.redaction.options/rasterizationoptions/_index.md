---
title: "RasterizationOptions"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Menyediakan opsi untuk mengonversi file menjadi PDF."
type: docs
weight: 420
url: /id/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Menyediakan opsi untuk mengonversi file menjadi PDF.

```csharp
public class RasterizationOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Menginisialisasi sebuah instance baru. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Mendapatkan atau mengatur tingkat Kepatuhan PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah semua halaman dalam dokumen perlu dikonversi menjadi gambar dan dimasukkan ke dalam satu file PDF. TRUE secara default, atur menjadi FALSE untuk menghindari rasterisasi. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Mendapatkan indikator yang bernilai true jika opsi rasterisasi lanjutan telah diatur. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Mendapatkan atau mengatur jumlah halaman yang akan dikonversi menjadi PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Mendapatkan atau mengatur indeks halaman pertama (berbasis 0) yang akan dikonversi menjadi PDF. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan. |

### Catatan

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Contoh

Contoh berikut menunjukkan cara mengatur opsi untuk proses rasterisasi.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // redaksi data sensitif pada slide pertama 
    
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

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi lanjutan border dengan pengaturan khusus.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan border khusus
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi lanjutan noise dengan pengaturan khusus.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan jumlah dan ukuran efek noise khusus
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Contoh berikut menunjukkan cara menerapkan opsi rasterisasi lanjutan tilt dengan pengaturan khusus.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Simpan dokumen dengan efek tilt khusus
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Lihat Juga

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
