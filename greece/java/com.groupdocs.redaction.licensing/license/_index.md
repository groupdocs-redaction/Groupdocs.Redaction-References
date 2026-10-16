---
title: "Άδεια"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει μεθόδους για την άδεια του στοιχείου."
type: docs
weight: 10
url: /el/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Παρέχει μεθόδους για την αδειοδότηση του στοιχείου. Μάθετε περισσότερα για την αδειοδότηση
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [License()](#License--) | Δημιουργήστε την Άδεια |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Αδειοδοτεί το στοιχείο. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Αδειοδοτεί το στοιχείο. |
|
### License() {#License--}
```
public License()
```


Δημιουργήστε την Άδεια


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Αδειοδοτεί το στοιχείο.

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | licensePath | java.lang.String | Η διαδρομή της άδειας. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Αδειοδοτεί το στοιχείο.

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Η ροή της άδειας. |
|

