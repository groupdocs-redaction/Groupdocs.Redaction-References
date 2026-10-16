---
title: "Redactor"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Mewakili kelas utama yang mengontrol proses redaksi dokumen, memungkinkan membuka, meredaksi, dan menyimpan dokumen."
type: docs
weight: 820
url: /id/net/groupdocs.redaction/redactor/
---
## Redactor class

Mewakili kelas utama yang mengontrol proses redaksi dokumen, memungkinkan membuka, meredaksi, dan menyimpan dokumen.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) menggunakan aliran. |
| [Redactor](redactor#constructor_3)(string) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) menggunakan jalur file. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) untuk dokumen yang dilindungi kata sandi menggunakan aliran. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Menginisialisasi instance baru dari kelas [`Redactor`](../redactor) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya dan pengaturan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Menerapkan redaksi pada dokumen. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Menerapkan kebijakan redaksi pada dokumen. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Menerapkan sekumpulan redaksi pada dokumen. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Melepaskan sumber daya. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Menghasilkan gambar pratinjau halaman tertentu dalam format gambar yang diberikan. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Mendapatkan informasi umum tentang dokumen - ukuran, jumlah halaman, dll. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Menyimpan dokumen ke file. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Menyimpan dokumen ke aliran yang ditentukan. |

### Catatan

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Contoh

Contoh berikut menunjukkan penerapan satu redaksi pada dokumen.

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

Contoh berikut menunjukkan penerapan daftar redaksi pada dokumen.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... redaksi lain
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, jika setidaknya satu redaksi gagal
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

Contoh berikut menunjukkan cara menerapkan kebijakan redaksi ke semua file dalam folder masuk yang diberikan, dan menyimpan ke salah satu folder keluar — untuk file yang berhasil diperbarui dan yang gagal.

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

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
}
```

Contoh berikut menunjukkan cara menyimpan dokumen menggunakan SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Penyensoran dokumen berada di sini
       // ...
    
       // Simpan dokumen dengan opsi default (konversi halaman menjadi gambar, simpan sebagai PDF)
       redactor.Save();
    
       // Simpan dokumen dalam format asli menimpa file asli
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Simpan dokumen ke file "*_Redacted.*" dalam format asli
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Simpan dokumen ke "*_AnyText.*" (misalnya timestamp alih-alih "AnyText") dalam nama file tanpa rasterisasi
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Lihat Juga

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
