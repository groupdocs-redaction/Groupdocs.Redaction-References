---
title: Redactor
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Mewakili kelas utama yang mengontrol proses penyuntingan dokumen memungkinkan untuk membuka menyunting dan menyimpan dokumen.
type: docs
weight: 660
url: /id/net/groupdocs.redaction/redactor/
---
## Redactor class

Mewakili kelas utama yang mengontrol proses penyuntingan dokumen, memungkinkan untuk membuka, menyunting, dan menyimpan dokumen.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Menginisialisasi instance baru dari[`Redactor`](../redactor) kelas menggunakan stream. |
| [Redactor](redactor#constructor_3)(string) | Menginisialisasi instance baru dari[`Redactor`](../redactor) kelas menggunakan file path. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Menginisialisasi instance baru dari[`Redactor`](../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Menginisialisasi instance baru dari[`Redactor`](../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Menginisialisasi instance baru dari[`Redactor`](../redactor)kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Menginisialisasi instance baru dari[`Redactor`](../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan jalur dan pengaturannya. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Menerapkan redaksi pada dokumen. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Menerapkan kebijakan penyuntingan pada dokumen. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Menerapkan sekumpulan redaksi pada dokumen. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Merilis sumber daya. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Menghasilkan gambar pratinjau dari halaman tertentu dalam format gambar tertentu. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Mendapat informasi umum tentang dokumen - ukuran, jumlah halaman, dll. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Menyimpan dokumen ke file. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Menyimpan dokumen ke aliran, termasuk lokasi khusus. |

### Perkataan

**Belajarlah lagi**

* Detail lebih lanjut tentang menerapkan redaksi: [Dasar redaksi](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Topik redaksi lebih lanjut: [Penggunaan tingkat lanjut](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Contoh

Contoh berikut menunjukkan penerapan satu redaksi pada dokumen.

Contoh berikut menunjukkan penerapan daftar redaksi pada dokumen.

Contoh berikut menunjukkan cara menerapkan kebijakan redaksi untuk semua file dalam folder masuk tertentu, dan menyimpan ke salah satu folder keluar - untuk file yang berhasil diperbarui dan yang gagal.

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

Contoh berikut menunjukkan cara menyimpan dokumen menggunakan SaveOptions.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... redaksi lainnya
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // salah, jika setidaknya satu redaksi gagal
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita bisa menggunakan document instance untuk melakukan redaksi
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Penyuntingan dokumen ada di sini
       // ...
    
       // Simpan dokumen dengan opsi default (konversi halaman menjadi gambar, simpan sebagai PDF)
       redactor.Save();
    
       // Simpan dokumen dalam format asli menimpa file asli
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Simpan dokumen ke file "*_Redacted.*" dalam format aslinya
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Simpan dokumen ke "*_AnyText.*" (mis. timestamp alih-alih "AnyText") dalam nama filenya tanpa rasterisasi
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Lihat juga

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* ruang nama [GroupDocs.Redaction](../../groupdocs.redaction)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
