---
title: "AddAdvancedOption"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan."
type: docs
weight: 70
url: /id/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll.) |

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

### Lihat Juga

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Anda dapat menggunakan metode ini untuk mendaftarkan opsi rasterisasi lanjutan yang akan diterapkan.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll.) |
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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
