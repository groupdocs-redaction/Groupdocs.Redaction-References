---
title: Load
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Memuat instance dariRedactionPolicygroupdocs.redaction/redactionpolicy dari jalur file.
type: docs
weight: 20
url: /id/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Memuat instance dari[`RedactionPolicy`](../../redactionpolicy) dari jalur file.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file XML |

### Nilai Pengembalian

Kebijakan redaksi

### Contoh

Contoh berikut menunjukkan cara menerapkan kebijakan redaksi untuk semua file dalam folder masuk tertentu, dan menyimpan ke salah satu folder keluar - untuk file yang berhasil diperbarui dan yang gagal.

Contoh berikut berisi file kebijakan XML sampel dengan konfigurasi sampel untuk semua jenis redaksi.

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Lihat juga

* class [RedactionPolicy](../../redactionpolicy)
* ruang nama [GroupDocs.Redaction](../../redactionpolicy)
* perakitan [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Memuat instance dari[`RedactionPolicy`](../../redactionpolicy) dari aliran.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| input | Stream | Aliran yang berisi konfigurasi XML |

### Nilai Pengembalian

Kebijakan redaksi

### Contoh

Contoh berikut menunjukkan cara menerapkan kebijakan redaksi untuk semua file dalam folder masuk tertentu, dan menyimpan ke salah satu folder keluar - untuk file yang berhasil diperbarui dan yang gagal.

Contoh berikut berisi file kebijakan XML sampel dengan konfigurasi sampel untuk semua jenis redaksi.

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Lihat juga

* class [RedactionPolicy](../../redactionpolicy)
* ruang nama [GroupDocs.Redaction](../../redactionpolicy)
* perakitan [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
