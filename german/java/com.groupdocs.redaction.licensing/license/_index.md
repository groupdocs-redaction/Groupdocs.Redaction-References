---
title: "Lizenz"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Methoden bereit, um die Komponente zu lizenzieren."
type: docs
weight: 10
url: /de/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Stellt Methoden zum Lizenzieren der Komponente bereit. Erfahren Sie mehr über Lizenzierung
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [License()](#License--) | Instanziiere die Lizenz |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Lizenziert die Komponente. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Lizenziert die Komponente. |
|
### License() {#License--}
```
public License()
```


Instanziiere die Lizenz


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Lizenziert die Komponente.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | licensePath | java.lang.String | Der Lizenzpfad. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Lizenziert die Komponente.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Der Lizenz-Stream. |
|

