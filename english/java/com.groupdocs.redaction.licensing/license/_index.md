---
title: License
second_title: GroupDocs.Redaction for Java API Reference
description: Provides methods for applying license.
type: docs
weight: 16
url: /java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Provides methods for applying license.

--------------------

**Learn more**

 *  More about licensing: [GroupDocs Licensing FAQ][]
 *  More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing][]

The following example demonstrates how to set the license for GroupDocs.Redaction.

```

  com.groupdocs.redaction.License license = new com.groupdocs.redaction.License();
 // as an alternative you can use a stream:
 license.setLicense(licensePath);
 
```


[GroupDocs Licensing FAQ]: https://purchase.groupdocs.com/faqs/licensing
[Evaluation Limitations and Licensing]: https://docs.groupdocs.com/redaction/java/evaluation-limitations-and-licensing/
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initialize an instance of License class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(String licensePath)](#setLicense-java.lang.String-) | Sets the GroupDocs.Redaction license from a file path. |
| [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Sets the GroupDocs.Redaction license from a stream. |
### License() {#License--}
```
public License()
```


Initialize an instance of License class.

### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Sets the GroupDocs.Redaction license from a file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licensePath | java.lang.String | License file path. |

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Sets the GroupDocs.Redaction license from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseStream | java.io.InputStream | License stream. |

