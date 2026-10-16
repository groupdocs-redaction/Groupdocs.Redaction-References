---
title: "Load"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Memuat sebuah instance dari RedactionPolicygroupdocs.redaction/redactionpolicy dari jalur file."
type: docs
weight: 20
url: /id/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Memuat sebuah instance dari [`RedactionPolicy`](../../redactionpolicy) dari jalur file.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file XML |

### Nilai Kembali

Kebijakan Redaction

### Contoh

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

Contoh berikut berisi file kebijakan XML contoh dengan konfigurasi contoh untuk semua jenis redaksi.

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

### Lihat Juga

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Memuat sebuah instance dari [`RedactionPolicy`](../../redactionpolicy) dari aliran.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| input | Stream | Aliran yang berisi konfigurasi XML |

### Nilai Kembali

Kebijakan Redaction

### Contoh

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

Contoh berikut berisi file kebijakan XML contoh dengan konfigurasi contoh untuk semua jenis redaksi.

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

### Lihat Juga

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
