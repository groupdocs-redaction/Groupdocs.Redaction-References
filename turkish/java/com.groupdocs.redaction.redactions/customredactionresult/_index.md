---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir sonuç döndüren temsili."
type: docs
weight: 14
url: /tr/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Bir sonuç döndüren [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) temsili.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getApply()](#getApply--) | Değiştirmenin uygulanıp uygulanmayacağını gösteren bir değer alır. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Değiştirmenin uygulanıp uygulanmayacağını gösteren bir değeri ayarlar. |
|
|  | [getText()](#getText--) | #getApply().getApply() olduğunda kullanılan değiştirme metnini alır |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | #getApply().getApply() olduğunda kullanılan değiştirme metnini ayarlar |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Değiştirmenin uygulanıp uygulanmayacağını gösteren bir değer alır.


**Returns:**
boolean -  true  eşleşen metni #getText().getText() ile değiştirmek için; aksi takdirde,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Değiştirmenin uygulanıp uygulanmayacağını gösteren bir değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | true  değiştirmeyi uygulamak için; aksi takdirde,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


#getApply().getApply() olduğunda kullanılan değiştirme metnini alır
true
.


**Returns:**
java.lang.String - Değiştirme metni.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


#getApply().getApply() olduğunda kullanılan değiştirme metnini ayarlar
true
.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Değiştirme metni. |
|

