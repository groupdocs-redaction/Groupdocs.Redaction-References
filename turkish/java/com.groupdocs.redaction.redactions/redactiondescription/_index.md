---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder."
type: docs
weight: 25
url: /tr/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisi olmadan başlatır. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisiyle başlatır. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | RedactionDescription sınıfının yeni bir örneğini, görüntü alanı değiştirme bilgisiyle başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Belgenin veri türünü alır - metin, meta veri veya ek açıklamalar. |
|
|  | [getActionType()](#getActionType--) | Kırpma işlemini alır: değiştirme, temizlik veya silme. |
|
|  | [getOriginalText()](#getOriginalText--) | Herhangi bir ifade sağlanmışsa, eşleşen metni alır. |
|
|  | [getReplacement()](#getReplacement--) | Değiştirme bilgisini alır, null olabilir. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Görüntü alanı kırpmaları için değiştirme bilgisini alır, metin kırpmaları için null döndürür. |
|
|  | [getDetails()](#getDetails--) | Kırpılan öğe için isteğe bağlı detay bilgisini alır. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Kırpılan öğe için isteğe bağlı detay bilgisini ayarlar. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisi olmadan başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redactionType | int | Kırpılan verinin türü |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Bu veriler üzerinde gerçekleştirilecek eylem |
|
|  | originalText | java.lang.String | Eşleşen metin, yorum veya ek açıklama gövdesi |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisiyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redactionType | int | Kırpılan verinin türü |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Bu veriler üzerinde gerçekleştirilecek eylem |
|
|  | originalText | java.lang.String | Eşleşen metin, yorum veya ek açıklama gövdesi |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Değiştirme metni, eşleşen metin ve orijinal dizedeki konumu |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


RedactionDescription sınıfının yeni bir örneğini, görüntü alanı değiştirme bilgisiyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redactionType | int | Kırpılan verinin türü |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Bu veriler üzerinde gerçekleştirilecek eylem |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Görüntü alanı değiştirme bilgisi |
|
|  | imageDetails | java.lang.String | Görüntünün metinsel açıklaması, varsayılan olarak String.Empty'dir |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Belgenin veri türünü alır - metin, meta veri veya ek açıklamalar.


**Returns:**
int - Belgenin veri türü - metin, meta veri veya ek açıklamalar.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Kırpma işlemini alır: değiştirme, temizlik veya silme.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Herhangi bir ifade sağlanmışsa, eşleşen metni alır.


**Returns:**
java.lang.String - Eşleşen metin, eğer bir ifade sağlanmışsa.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Değiştirme bilgisini alır, null olabilir.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Görüntü alanı kırpmaları için değiştirme bilgisini alır, metin kırpmaları için null döndürür.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Kırpılan öğe için isteğe bağlı detay bilgisini alır.


**Returns:**
java.lang.String - Kırpılan öğe için isteğe bağlı detay bilgisi.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Kırpılan öğe için isteğe bağlı detay bilgisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Kırpılan öğe için isteğe bağlı detay bilgisi. |
|

