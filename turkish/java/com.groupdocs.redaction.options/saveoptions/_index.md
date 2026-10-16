---
title: "SaveOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Çıktı dosya adını değiştirme ve/veya belgeyi görüntü tabanlı PDF rasterleştirmeye dönüştürme seçenekleri sağlar."
type: docs
weight: 14
url: /tr/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Çıktı dosya adını değiştirme ve/veya belgeyi görüntü tabanlı PDF'ye (tarama) dönüştürme seçenekleri sunar.

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Varsayılanlarla yeni bir örnek başlatır: PDF'ye rasterleştir - false, ek sonek ekle - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Verilen parametrelerle yeni bir örnek başlatır. |
|
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Varsayılan sonek değerini temsil eder, bu "Redacted". |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Kaydetmeden önce dosya adının değiştirilip değiştirilmesi gerektiğini gösteren bir değeri alır. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Kaydetmeden önce dosya adının değiştirilip değiştirilmesi gerektiğini gösteren bir değeri ayarlar. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Çıktı dosya adı için özel bir sonek alır. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Çıktı dosya adı için özel bir sonek ayarlar. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri alır. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri ayarlar. |
|
|  | [getRasterization()](#getRasterization--) | Rasterleştirme ayarlarını alır. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Kelime işlem kaydetme seçenekleri. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Varsayılanlarla yeni bir örnek başlatır: PDF'ye rasterleştir - false, ek sonek ekle - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Verilen parametrelerle yeni bir örnek başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, eğer belgedeki tüm sayfalar görüntülere dönüştürülüp tek bir PDF dosyasına konulması gerekiyorsa |
|
|  | suffix | java.lang.String | Bu metin dosya adının sonuna eklenecek, boş değilse ayrıca AddSuffix'i true olarak ayarlar |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Varsayılan sonek değerini temsil eder, bu "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Dosya adının kaydedilmeden önce değiştirilmesi gerekip gerekmediğini gösteren bir değeri alır. Varsayılan olarak False.


**Returns:**
boolean - Dosya adının kaydedilmeden önce değiştirilmesi gerekip gerekmediğini gösteren bir değer. Varsayılan olarak False.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Dosya adının kaydedilmeden önce değiştirilmesi gerekip gerekmediğini gösteren bir değeri ayarlar. Varsayılan olarak False.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Dosya adının kaydedilmeden önce değiştirilmesi gerekip gerekmediğini gösteren bir değer. Varsayılan olarak False. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Çıktı dosya adı için özel bir ek alır. Belirtilmemişse,
SaveSuffix
sabit kullanılacaktır.


**Returns:**
java.lang.String - Çıktı dosya adı için özel bir ek. Belirtilmemişse,  SaveSuffix  sabiti kullanılacaktır.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Çıktı dosya adı için özel bir ek ayarlar. Belirtilmemişse,
SaveSuffix
sabit kullanılacaktır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Çıktı dosya adı için özel bir ek. Belirtilmemişse,  SaveSuffix  sabiti kullanılacaktır. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri alır.


**Returns:**
boolean - Belgenin tüm sayfalarının görüntülere dönüştürülüp tek bir PDF dosyasına konulması gerekip gerekmediğini gösteren bir değer.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Belgenin tüm sayfalarının görüntülere dönüştürülüp tek bir PDF dosyasına konulması gerekip gerekmediğini gösteren bir değer. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Rasterleştirme ayarlarını alır.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Kelime işlem kaydetme seçenekleri.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
