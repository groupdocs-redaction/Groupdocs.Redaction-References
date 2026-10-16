---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Dosyaları PDF'ye dönüştürmek için seçenekler sağlar."
type: docs
weight: 12
url: /tr/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Dosyaları PDF'ye dönüştürmek için seçenekler sağlar.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Yeni bir örnek başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri alır. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri ayarlar. |
|
|  | [getPageIndex()](#getPageIndex--) | PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizinini alır. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizinini ayarlar. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | PageIndex özelliğinin başlatıldıktan sonra değiştirilip (ayarlanıp) değiştirildiğini gösteren bir değeri alır. |
|
|  | [getPageCount()](#getPageCount--) | PDF'ye dönüştürülecek sayfa sayısını alır. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | PDF'ye dönüştürülecek sayfa sayısını ayarlar. |
|
|  | [isPageCountSet()](#isPageCountSet--) | PageCount özelliğinin başlatıldıktan sonra değiştirilip (ayarlanıp) değiştirildiğini gösteren bir değeri alır. |
|
|  | [getCompliance()](#getCompliance--) | PDF Uyumluluk seviyesini alır. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | PDF Uyumluluk seviyesini ayarlar. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Gelişmiş rasterleştirme seçenekleri ayarlandıysa doğru olan bir göstergiyi alır. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Uygulanacak bir gelişmiş rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Uygulanacak bir gelişmiş rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Yeni bir örnek başlatır.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri alır. Varsayılan olarak TRUE, rasterleştirmeyi önlemek için FALSE olarak ayarlanır.


**Returns:**
boolean - Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değer. Varsayılan olarak TRUE, rasterleştirmeyi önlemek için FALSE olarak ayarlanır.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değeri ayarlar. Varsayılan olarak TRUE, rasterleştirmeyi önlemek için FALSE olarak ayarlanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına konulup konulmayacağını gösteren bir değer. Varsayılan olarak TRUE, rasterleştirmeyi önlemek için FALSE olarak ayarlanır. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizinini alır.


**Returns:**
int - PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizini.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizinini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) dizini. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


PageIndex özelliğinin başlatıldıktan sonra değiştirilip (ayarlanıp) değiştirildiğini gösteren bir değeri alır.


**Returns:**
boolean - PageIndex özelliğinin başlatıldıktan sonra değiştirilip (ayarlanıp) değiştirildiğini gösteren bir değer.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


PDF'ye dönüştürülecek sayfa sayısını alır.


**Returns:**
int - PDF'ye dönüştürülecek sayfa sayısı.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


PDF'ye dönüştürülecek sayfa sayısını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | PDF'ye dönüştürülecek sayfa sayısı. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


PageCount özelliğinin başlatıldıktan sonra değiştirilip (ayarlanıp) değiştirildiğini gösteren bir değeri alır.


**Returns:**
boolean - PageCount özelliğinin başlatıldıktan sonra değiştirildiğini (ayarlandığını) gösteren bir değer.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


PDF Uyumluluk seviyesini alır.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


PDF Uyumluluk seviyesini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF Uyumluluk seviyesi. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Gelişmiş rasterleştirme seçenekleri ayarlandıysa doğru olan bir göstergiyi alır.


**Returns:**
boolean - Gelişmiş rasterleştirme seçenekleri ayarlandığında doğru olan bir gösterge.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Uygulanacak bir gelişmiş rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar. |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Uygulanacak bir gelişmiş rasterleştirme seçeneğini kaydetmek için bu yöntemi kullanabilirsiniz.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar. |
|
|  | parametreler | java.util.HashMap<java.lang.String,java.lang.String> | Verilen efekt için parametreler, örneğin dönüş açısı |
|

