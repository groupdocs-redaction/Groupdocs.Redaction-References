---
title: "MetadataItem"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Tüm desteklenen formatlar için ortak olan ve meta veri redaksiyonlarında kullanılan bir meta veri öğesini temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Tüm desteklenen formatlar için ortak olan ve meta veri redaksiyonlarında kullanılan bir meta veri öğesini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Yeni bir örnek başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Belge içinde göründüğü gibi meta veri öğesinin özgün adını alır. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Belge içinde göründüğü gibi meta veri öğesinin özgün adını ayarlar. |
|
|  | [getCategory()](#getCategory--) | Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisini alır. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisini ayarlar. |
|
|  | [getFilter()](#getFilter--) | Şunun değerini alır |
MetadataFilters
, bu meta veri öğesine atanan ve öğe filtrelemede kullanılan.
|
|  | [setFilter(int value)](#setFilter-int-) | Şunun değerini ayarlar |
MetadataFilters
, bu meta veri öğesine atanan ve öğe filtrelemede kullanılan.
|
|  | [getValues()](#getValues--) | Meta veri öğesinin değerini alır. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Meta veri öğesinin değerini ayarlar. |
|
|  | [isCustom()](#isCustom--) | Bu öğenin özel olup olmadığını (belgenin yazarları tarafından eklenmiş) gösteren bir değeri alır. |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Bu öğenin özel olup olmadığını (belgenin yazarları tarafından eklenmiş) gösteren bir değeri ayarlar. |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | OriginalName ve diğer verileri kullanarak , için bir sözlük anahtarı alır. |
|
|  | [createClone()](#createClone--) | Mevcut örneğin derin bir klonunu oluşturur. |
|
|  | [getActualValue()](#getActualValue--) | Meta veri öğesi değerinin dize temsili alır. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Yeni bir örnek başlatır.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Belge içinde göründüğü gibi meta veri öğesinin özgün adını alır.


**Returns:**
java.lang.String - Belge içinde göründüğü gibi meta veri öğesinin özgün adı.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Belge içinde göründüğü gibi meta veri öğesinin özgün adını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Belge içinde göründüğü gibi meta veri öğesinin özgün adı. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisini alır.


**Returns:**
java.lang.String - Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisi.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Örneğin gömülü bir kaynak meta veri öğesi için kaynak kimliği gibi meta veri öğesinin bir kategorisi. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Şunun değerini alır
MetadataFilters
, bu meta veri öğesine atanan ve öğe filtrelemede kullanılan.


**Returns:**
int - MetadataFilters'in bir değeri, bu meta veri öğesine atanmış ve öğe filtrelemede kullanılır.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Şunun değerini ayarlar
MetadataFilters
, bu meta veri öğesine atanan ve öğe filtrelemede kullanılan.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | MetadataFilters'in bir değeri, bu meta veri öğesine atanmış ve öğe filtrelemede kullanılır. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Meta veri öğesinin değerini alır.


**Returns:**
java.util.List<java.lang.String> - Meta veri öğesi değeri.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Meta veri öğesinin değerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.util.List<java.lang.String> | Meta veri öğesi değeri. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Bu öğenin özel olup olmadığını (belgenin yazarları tarafından eklenmiş) gösteren bir değeri alır.


**Returns:**
boolean - Bu öğenin özel olup olmadığını gösteren değer (belgenin yazarları tarafından eklenmiştir).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Bu öğenin özel olup olmadığını (belgenin yazarları tarafından eklenmiş) gösteren bir değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Bu öğenin özel olup olmadığını gösteren değer (belgenin yazarları tarafından eklenmiştir). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


OriginalName ve diğer verileri kullanarak , için bir sözlük anahtarı alır.


**Returns:**
java.lang.String - , için bir sözlük anahtarı, OriginalName ve diğer verileri kullanarak.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Mevcut örneğin derin bir klonunu oluşturur.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Meta veri öğesi değerinin dize temsili alır.


**Returns:**
java.lang.String - Meta veri öğesi değerinin dize temsili.

