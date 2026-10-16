---
title: "लाइसेंस"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "कम्पोनेंट को लाइसेंस करने के लिए मेथड्स प्रदान करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

घटक को लाइसेंस करने के लिए विधियाँ प्रदान करता है। लाइसेंसिंग के बारे में अधिक जानें
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [License()](#License--) | लाइसेंस को इंस्टैंसिएट करें |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | घटक को लाइसेंस करता है। |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | घटक को लाइसेंस करता है। |
|
### License() {#License--}
```
public License()
```


लाइसेंस को इंस्टैंसिएट करें


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


घटक को लाइसेंस करता है।

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | licensePath | java.lang.String | लाइसेंस पथ। |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


घटक को लाइसेंस करता है।

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | लाइसेंस स्ट्रीम। |
|

