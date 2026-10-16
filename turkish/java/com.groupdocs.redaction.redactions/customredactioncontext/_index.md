---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Giriş verilerini sağlar."
type: docs
weight: 13
url: /tr/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Giriş verilerini sağlar [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) için.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Eşleşen parçanın sayfa numarasını, mevcut olduğunda alır. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Eşleşen parçanın sayfa numarasını ayarlar. |
|
|  | [getText()](#getText--) | Kırpma için eşleşen metni alır. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Kırpma için eşleşen metni ayarlar. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Eşleşen parçanın sayfa numarasını, mevcut olduğunda alır.


**Returns:**
int - Sayfa numarası veya sayfa bilinmiyorsa biçime özgü bir değer.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Eşleşen parçanın sayfa numarasını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Sayfa numarası. |
|

### getText() {#getText--}
```
public final String getText()
```


Kırpma için eşleşen metni alır.


**Returns:**
java.lang.String - Eşleşen metin.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Kırpma için eşleşen metni ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Eşleşen metin. |
|

