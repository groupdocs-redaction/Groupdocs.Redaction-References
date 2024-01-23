---
title: License
second_title: GroupDocs.Redaction for Java API Reference
description: Provides methods to license the component.
type: docs
weight: 10
url: /java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Provides methods to license the component. Learn more about licensing  [here][] .


[here]: https://purchase.groupdocs.com/faqs/licensing
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Instantiate the License |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(String licensePath)](#setLicense-java.lang.String-) | Licenses the component. |
| [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Instantiate the License

### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Licenses the component.

--------------------

> ```
> The following example demonstrates how to set a license
>  passing a path to the license file.
>  
>  string licensePath = "GroupDocs.Signature.lic";
>  GroupDocs.Signature.License lic = new GroupDocs.Signature.License();
>  lic.SetLicense(licensePath);
> ```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licensePath | java.lang.String | The license path. |

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Licenses the component.

--------------------

> ```
> The following example demonstrates how to set a license
>  passing Stream of the license file.
>  
>  using (FileStream licenseStream = new FileStream("GroupDocs.Signature.lic", FileMode.Open))
>  {
>      GroupDocs.Signature.License lic = new GroupDocs.Signature.License();
>      lic.SetLicense(licenseStream);
>  }
> ```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseStream | java.io.InputStream | The license stream. |

