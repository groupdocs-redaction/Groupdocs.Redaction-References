---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Eşleşen metin değişimi için seçenekleri temsil eder."
type: docs
weight: 31
url: /tr/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Eşleşen metin değişimi için seçenekleri temsil eder.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | ReplacementOptions sınıfının yeni bir örneğini, değiştirme metni bir seçenek olarak kullanarak başlatır. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | ReplacementOptions sınıfının yeni bir örneğini, renkli dikdörtgen bir seçenek olarak kullanarak başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getActionType()](#getActionType--) | Değiştirme eylemini alır: kutu çiz veya metni değiştir. |
|
|  | [getReplacement()](#getReplacement--) | Metinsel değiştirme değerini alır. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Metinsel değiştirme değerini ayarlar. |
|
|  | [getBoxColor()](#getBoxColor--) | Bir öğe için rengi alır |
ReplacementType.DrawBox
seçenek (aksi takdirde yok sayılır).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Bir öğe için rengi ayarlar |
ReplacementType.DrawBox
seçenek (aksi takdirde yok sayılır).
|
|  | [getFilters()](#getFilters--) | Bu kırpma ile uygulanacak filtrelerin bir dizisini alır. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Bu kırpma ile uygulanacak filtrelerin bir dizisini ayarlar. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Özel bir kırpma işleyicisini alır. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Özel bir kırpma işleyicisini ayarlar. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


ReplacementOptions sınıfının yeni bir örneğini, değiştirme metni bir seçenek olarak kullanarak başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değiştirme | java.lang.String | Metinsel değiştirme |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


ReplacementOptions sınıfının yeni bir örneğini, renkli dikdörtgen bir seçenek olarak kullanarak başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | renk | java.awt.Color | Dikdörtgen rengi |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Değiştirme eylemini alır: kutu çiz veya metni değiştir.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Metinsel değiştirme değerini alır.


**Returns:**
java.lang.String - Metinsel değiştirme değeri.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Metinsel değiştirme değerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Metinsel değiştirme değeri. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Bir öğe için rengi alır
ReplacementType.DrawBox
seçenek (aksi takdirde yok sayılır).


**Returns:**
java.awt.Color - Bir  ReplacementType.DrawBox  seçeneği için renk (aksi takdirde yok sayılır).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Bir öğe için rengi ayarlar
ReplacementType.DrawBox
seçenek (aksi takdirde yok sayılır).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.awt.Color | ReplacementType.DrawBox seçeneği için renk (aksi takdirde yok sayılır). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Bu kırpma ile uygulanacak filtrelerin bir dizisini alır.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Bu redaksiyonla uygulanacak filtrelerin bir dizisi.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Bu kırpma ile uygulanacak filtrelerin bir dizisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Bu redaksiyonla uygulanacak filtrelerin bir dizisi. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Özel bir redaksiyon işleyicisi alır. Yalnızca PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) için desteklenir.


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Özel bir redaksiyon işleyicisi ayarlar. Yalnızca PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) için desteklenir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) bir örnek. |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
