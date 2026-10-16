---
title: "Licens"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller metoder för att licensiera komponenten."
type: docs
weight: 10
url: /sv/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Tillhandahåller metoder för att licensiera komponenten. Läs mer om licensiering
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [License()](#License--) | Instansiera licensen |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Licensierar komponenten. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Licensierar komponenten. |
|
### License() {#License--}
```
public License()
```


Instansiera licensen


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Licensierar komponenten.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | licensePath | java.lang.String | Licenssökvägen. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Licensierar komponenten.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Licensströmmen. |
|

