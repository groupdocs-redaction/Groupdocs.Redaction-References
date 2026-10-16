---
title: "Licentie"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt methoden om het component te licentiëren."
type: docs
weight: 10
url: /nl/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Biedt methoden om het component te licentiëren. Meer informatie over licenties
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [License()](#License--) | Instantieer de licentie |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Licentieert het component. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Licentieert het component. |
|
### License() {#License--}
```
public License()
```


Instantieer de licentie


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Licentieert het component.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | licensePath | java.lang.String | Het licentiepad. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Licentieert het component.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | De licentiestroom. |
|

