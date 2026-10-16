---
title: "Lisans"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bileşeni lisanslamak için yöntemler sağlar."
type: docs
weight: 10
url: /tr/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Bileşeni lisanslamak için yöntemler sağlar. Lisanslama hakkında daha fazla bilgi edinin
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [License()](#License--) | Lisansı örnekleyin |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Bileşeni lisanslar. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Bileşeni lisanslar. |
|
### License() {#License--}
```
public License()
```


Lisansı örnekleyin


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Bileşeni lisanslar.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | licensePath | java.lang.String | Lisans yolu. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Bileşeni lisanslar.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Lisans akışı. |
|

