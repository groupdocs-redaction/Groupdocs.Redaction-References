---
title: "Lisensi"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan metode untuk melisensikan komponen."
type: docs
weight: 10
url: /id/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Menyediakan metode untuk melisensikan komponen. Pelajari lebih lanjut tentang pelisensian
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [License()](#License--) | Instansiasi Lisensi |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Melisensikan komponen. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Melisensikan komponen. |
|
### License() {#License--}
```
public License()
```


Instansiasi Lisensi


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Melisensikan komponen.

<br />

*** ** * ** ***

> ```
>  The following example demonstrates how to set a license
>  passing a path to the license file.
>   string licensePath = "GroupDocs.Signature.lic";
>  GroupDocs.Signature.License lic = new GroupDocs.Signature.License();
>  lic.SetLicense(licensePath);
>  
>  
> ```

<br />



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | licensePath | java.lang.String | Jalur lisensi. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Melisensikan komponen.

<br />

*** ** * ** ***

> ```
>  The following example demonstrates how to set a license
>  passing Stream of the license file.
>   using (FileStream licenseStream = new FileStream("GroupDocs.Signature.lic", FileMode.Open))
>  {
>      GroupDocs.Signature.License lic = new GroupDocs.Signature.License();
>      lic.SetLicense(licenseStream);
>  }
>  
>  
> ```

<br />



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Aliran lisensi. |
|

