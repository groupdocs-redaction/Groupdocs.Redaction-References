---
title: "许可证"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供对组件进行授权的方法。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

提供对组件授权的方法。了解更多关于授权的信息
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [License()](#License--) | 实例化许可证 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | 为组件授权。 |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | 为组件授权。 |
|
### License() {#License--}
```
public License()
```


实例化许可证


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


为组件授权。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | licensePath | java.lang.String | 许可证路径。 |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


为组件授权。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | 许可证流。 |
|

