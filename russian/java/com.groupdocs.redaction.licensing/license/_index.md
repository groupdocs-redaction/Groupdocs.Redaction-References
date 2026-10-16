---
title: "Лицензия"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет методы для лицензирования компонента."
type: docs
weight: 10
url: /ru/java/com.groupdocs.redaction.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

Предоставляет методы лицензирования компонента. Узнайте больше о лицензировании
[here](../https://purchase.groupdocs.com/faqs/licensing)
.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [License()](#License--) | Создайте экземпляр лицензии |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [setLicense(String licensePath)](#setLicense-java.lang.String-) | Лицензирует компонент. |
|
|  | [setLicense(InputStream licenseStream)](#setLicense-java.io.InputStream-) | Лицензирует компонент. |
|
### License() {#License--}
```
public License()
```


Создайте экземпляр лицензии


### setLicense(String licensePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String licensePath)
```


Лицензирует компонент.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | licensePath | java.lang.String | Путь к лицензии. |
|

### setLicense(InputStream licenseStream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream licenseStream)
```


Лицензирует компонент.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | licenseStream | java.io.InputStream | Поток лицензии. |
|

