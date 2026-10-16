---
title: "ReplacementType"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Eşleşen metin için bir değiştirme türünü temsil eder."
type: docs
weight: 38
url: /tr/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Eşleşen metin için bir değiştirme türünü temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Eşleşen metni başka bir dizeyle değiştirir, örn. |
|
|  | [DrawBox](#DrawBox) | Kırpılmış metin yerine belirli bir renkte (Varsayılan olarak Siyah) bir dikdörtgen çizer. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Eşleşen metni başka bir dizeyle değiştirir, örn. muafiyet kodu.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Kırpılmış metin yerine belirli bir renkte (Varsayılan olarak Siyah) bir dikdörtgen çizer.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
