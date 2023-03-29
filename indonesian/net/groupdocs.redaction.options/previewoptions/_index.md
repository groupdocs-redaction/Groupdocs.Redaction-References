---
title: PreviewOptions
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Menyediakan opsi untuk menetapkan persyaratan dan streaming delegasi untuk pembuatan pratinjau.
type: docs
weight: 330
url: /id/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Menyediakan opsi untuk menetapkan persyaratan dan streaming delegasi untuk pembuatan pratinjau.

```csharp
public class PreviewOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Menginisialisasi instance baru dari kelas PreviewOptions, menyebabkan aliran keluaran ditutup. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Menginisialisasi instance baru dari kelas PreviewOptions, menyebabkan aliran output dikembalikan ke klien untuk digunakan lebih lanjut. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Mendapat atau menyetel instance delegasi pembuatan aliran halaman. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Mendapat atau menyetel tinggi pratinjau halaman. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Mendapat atau menyetel larik nomor halaman untuk menghasilkan pratinjau. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Mendapat atau mengatur format gambar pratinjau. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Mendapat atau menyetel instance delegasi penyelesaian pratinjau halaman. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Mendapat atau menyetel lebar pratinjau halaman. |

### Contoh

Contoh berikut menunjukkan cara mendapatkan pratinjau dokumen menggunakan[`PreviewOptions`](../previewoptions) Dan[`CreatePageStream`](./createpagestream) melimpahkan.

Contoh berikut menunjukkan cara mendapatkan pratinjau dokumen menggunakan[`PreviewOptions`](../previewoptions) dan kedua delegasi.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    var previewOptions = new PreviewOptions(createDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // lakukan apa saja dengan Stream, berisi pratinjau halaman
        pageStream.Close();
    };
    var previewOptions = new PreviewOptions(createDelegate, releaseDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

### Lihat juga

* ruang nama [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->