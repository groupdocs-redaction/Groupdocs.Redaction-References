---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redaksiyon tamamlama durumunu temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Redaksiyon tamamlama durumunu temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Applied](#Applied) | Redaction tamamen ve başarılı bir şekilde uygulandı. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redaction yalnızca eşleşmelerinin bir kısmına uygulandı. |
|
|  | [Skipped](#Skipped) | Kırpma atlandı (uygulanmadı). |
|
|  | [Failed](#Failed) | Kırpma bir istisna ile başarısız oldu. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redaction tamamen ve başarılı bir şekilde uygulandı.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redaction yalnızca eşleşmelerinin bir kısmına uygulandı.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Kırpma atlandı (uygulanmadı).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Kırpma bir istisna ile başarısız oldu.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
