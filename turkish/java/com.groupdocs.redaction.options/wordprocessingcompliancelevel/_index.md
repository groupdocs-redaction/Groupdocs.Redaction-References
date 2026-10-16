---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Kelime işlem belgeleri için OOXML uyumluluk seviyeleri."
type: docs
weight: 22
url: /tr/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

Word processing belgeleri için OOXML uyumluluk seviyeleri. Strict yalnızca Transitional seviyesine düşürülebilir, Ecma'ya düşürülemez.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 1st Edition, 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 1st Edition, 2006.


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional.


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict.


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
