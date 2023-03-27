---
title: AddAdvancedOption
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan untuk diterapkan.
type: docs
weight: 70
url: /id/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan untuk diterapkan.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Memberikan informasi tentang jenis efek yang dipilih (grayscale, border, dll.) |

### Contoh

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

### Lihat juga

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* ruang nama [GroupDocs.Redaction.Options](../../rasterizationoptions)
* perakitan [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan untuk diterapkan.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Memberikan informasi tentang jenis efek yang dipilih (grayscale, border, dll.) |
| parameters | Dictionary`2 | Parameter untuk efek yang diberikan, seperti sudut rotasi |

### Contoh

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* ruang nama [GroupDocs.Redaction.Options](../../rasterizationoptions)
* perakitan [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
