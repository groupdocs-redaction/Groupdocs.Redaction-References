---
title: "Licenza"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce metodi per licenziare il componente."
type: docs
weight: 10
url: /it/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Fornisce metodi per licenziare il componente. Scopri di più sulla licenza
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [License()](#License--) | Istanzia la Licenza |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Licenzia il componente. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Licenzia il componente. |
|
### License() {#License--}
```
public License()
```


Istanzia la Licenza


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Licenzia il componente.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | licensePath | java.lang.String | Il percorso della licenza. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Licenzia il componente.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Il flusso della licenza. |
|

