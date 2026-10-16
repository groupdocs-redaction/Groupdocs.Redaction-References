---
title: "라이선스"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "구성 요소에 라이선스를 적용하는 메서드를 제공합니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

구성 요소에 라이선스를 적용하기 위한 메서드를 제공합니다. 라이선스에 대해 자세히 알아보세요
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [License()](#License--) | 라이선스를 인스턴스화합니다 |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | 구성 요소에 라이선스를 적용합니다. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | 구성 요소에 라이선스를 적용합니다. |
|
### License() {#License--}
```
public License()
```


라이선스를 인스턴스화합니다


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


구성 요소에 라이선스를 적용합니다.

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | licensePath | java.lang.String | 라이선스 경로. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


구성 요소에 라이선스를 적용합니다.

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | 라이선스 스트림. |
|

