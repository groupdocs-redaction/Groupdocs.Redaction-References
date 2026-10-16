---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redaksiyon gerçekleştirmek için alınabilecek eylemleri temsil eder."
type: docs
weight: 37
url: /tr/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Redaksiyon gerçekleştirmek için alınabilecek eylemleri temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Replacement](#Replacement) | Kırpılmış metin başka bir metinle değiştirildi veya bir blokla kapatıldı. |
|
|  | [Cleanup](#Cleanup) | Veriler kaldırıldı, ancak belgede boş bir nesne kalır. |
|
|  | [Deletion](#Deletion) | Veriler ve ilgili yapılar belgeden kaldırıldı. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Kırpılmış metin başka bir metinle değiştirildi veya bir blokla kapatıldı.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Veriler kaldırıldı, ancak belgede boş bir nesne kalır.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Veriler ve ilgili yapılar belgeden kaldırıldı.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
