---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belge meta verilerinin en yaygın türlerinin bir listesini temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Belge meta verilerinin en yaygın türlerinin bir listesini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [None](#None) | Boş filtre ayarı, hiçbir meta veri öğesiyle eşleşmez. |
|
|  | [Author](#Author) | Belgenin yazarı. |
|
|  | [Category](#Category) | Belgenin kategorisi. |
|
|  | [Comments](#Comments) | Belge için yorum. |
|
|  | [Company](#Company) | Yazarın şirketi. |
|
|  | [ContentStatus](#ContentStatus) | İçerik durumu. |
|
|  | [CreatedTime](#CreatedTime) | Oluşturulma zamanı. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Köprü temeli. |
|
|  | [LastPrinted](#LastPrinted) | Son yazdırma tarihi ve saati. |
|
|  | [LastSavedBy](#LastSavedBy) | Son kaydetme kullanıcı tarafından. |
|
|  | [LastSavedTime](#LastSavedTime) | Son kaydetme tarihi ve saati. |
|
|  | [NameOfApplication](#NameOfApplication) | Belgenin oluşturulduğu uygulamanın adı. |
|
|  | [Manager](#Manager) | Yazarın yöneticisinin adı. |
|
|  | [RevisionNumber](#RevisionNumber) | Revizyon numarası. |
|
|  | [Subject](#Subject) | Belgenin konusu. |
|
|  | [Template](#Template) | Belge şablonu adı. |
|
|  | [Title](#Title) | Belge başlığı. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Toplam düzenleme süresi. |
|
|  | [Version](#Version) | Belgenin sürümü. |
|
|  | [Description](#Description) | Belgenin açıklaması. |
|
|  | [Keywords](#Keywords) | Belgenin anahtar kelimeleri. |
|
|  | [ContentType](#ContentType) | İçerik türü. |
|
|  | [All](#All) | Meta veri öğelerinin tüm türleri. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getNames()](#getNames--) | Tüm bildirilen filtre türlerini içeren bir küme alır. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | MetadataFiler değerini adıyla alır. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Virgülle ayrılmış MetadataFilers değerleri içeren bir dizeyi tamsayıya ayrıştırır. |
|
|  | [toString(int value)](#toString-int-) | Tamsayıyı virgülle ayrılmış MetadataFilers değerleri içeren bir dize olarak kaydeder. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Boş filtre ayarı, hiçbir meta veri öğesiyle eşleşmez.


### Author {#Author}
```
public static final int Author
```


Belgenin yazarı.


### Category {#Category}
```
public static final int Category
```


Belgenin kategorisi.


### Comments {#Comments}
```
public static final int Comments
```


Belge için yorum.


### Company {#Company}
```
public static final int Company
```


Yazarın şirketi.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


İçerik durumu.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Oluşturulma zamanı.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Köprü temeli.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Son yazdırma tarihi ve saati.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Son kaydetme kullanıcı tarafından.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Son kaydetme tarihi ve saati.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Belgenin oluşturulduğu uygulamanın adı.


### Manager {#Manager}
```
public static final int Manager
```


Yazarın yöneticisinin adı.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Revizyon numarası.


### Subject {#Subject}
```
public static final int Subject
```


Belgenin konusu.


### Template {#Template}
```
public static final int Template
```


Belge şablonu adı.


### Title {#Title}
```
public static final int Title
```


Belge başlığı.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Toplam düzenleme süresi.


### Version {#Version}
```
public static final int Version
```


Belgenin sürümü.


### Description {#Description}
```
public static final int Description
```


Belgenin açıklaması.


### Keywords {#Keywords}
```
public static final int Keywords
```


Belgenin anahtar kelimeleri.


### ContentType {#ContentType}
```
public static final int ContentType
```


İçerik türü.


### All {#All}
```
public static final int All
```


Meta veri öğelerinin tüm türleri.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Tüm bildirilen filtre türlerini içeren bir küme alır.


**Returns:**
java.util.Set<java.lang.String> - Tüm bildirilen filtre türlerini içeren bir küme.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


MetadataFiler değerini adıyla alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | valueName | java.lang.String | MetadataFilter adı. |
|

**Returns:**
int - MetadataFiler değeri.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Virgülle ayrılmış MetadataFilers değerleri içeren bir dizeyi tamsayıya ayrıştırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | values | java.lang.String | Virgülle ayrılmış MetadataFilers değerleri içeren bir dize. |
|

**Returns:**
int - MetadataFilers değeri.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Tamsayıyı virgülle ayrılmış MetadataFilers değerleri içeren bir dize olarak kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | MetadataFiler değeri. |
|

**Returns:**
java.lang.String - Virgülle ayrılmış MetadataFiler değerleri içeren bir dize.

