---
title: "RedactionResult"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redaksiyon işleminin sonucunu temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Redaksiyon işleminin sonucunu temsil eder.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getStatus()](#getStatus--) | Yürütme durumunu alır. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Tanılamalar için hata mesajını alır. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | RedactionResult sınıfının yeni bir örneğini Skipped durumu ile başlatır. |
|
|  | [partial(String description)](#partial-java.lang.String-) | RedactionResult sınıfının yeni bir örneğini PartiallyApplied durumu ile başlatır. |
|
|  | [failed(String description)](#failed-java.lang.String-) | RedactionResult sınıfının yeni bir örneğini Failed durumu ile başlatır. |
|
|  | [successful()](#successful--) | RedactionResult sınıfının yeni bir örneğini Applied (successful) durumu ile başlatır. |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Yürütme durumunu alır.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Tanılamalar için hata mesajını alır.


**Returns:**
java.lang.String - Tanılamalar için hata mesajı.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


RedactionResult sınıfının yeni bir örneğini Skipped durumu ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | açıklama | java.lang.String | İşlemin atlanma nedeni |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


RedactionResult sınıfının yeni bir örneğini PartiallyApplied durumu ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | açıklama | java.lang.String | İşlemin tam olarak uygulanmama nedeni |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


RedactionResult sınıfının yeni bir örneğini Failed durumu ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | açıklama | java.lang.String | Hata veya istisna ayrıntıları |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


RedactionResult sınıfının yeni bir örneğini Applied (successful) durumu ile başlatır.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

