---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Kelime işlem kaydetme seçenekleri."
type: docs
weight: 15
url: /tr/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Kelime işlem kaydetme seçenekleri.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Kaydetme sırasında uygulanacak OOXML uyumluluğu. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


Kaydetme sırasında uygulanacak OOXML uyumluluğu.  null  orijinal belge seviyesini korur. Strict doğrudan Ecma olarak kaydedilemez; önce Transitional kullanın.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

