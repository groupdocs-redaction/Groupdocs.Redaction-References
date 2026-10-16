---
title: "Redactor"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belge redaksiyon sürecini kontrol eden, belgeleri açma, redakte etme ve kaydetme imkanı sağlayan ana sınıfı temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Belge redaksiyon sürecini kontrol eden, belgeleri açmaya, redakte etmeye ve kaydetmeye izin veren ana sınıfı temsil eder.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Yeni bir örnek oluşturur |
Redactor
dosya yolu kullanan sınıf.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Yeni bir örnek oluşturur |
Redactor
akış kullanan sınıf.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Yeni bir örnek oluşturur |
Redactor
yolunu kullanan şifre korumalı bir belge için sınıf.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Yeni bir örnek oluşturur |
Redactor
yolunu ve ayarlarını kullanan şifre korumalı bir belge için sınıf.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Yeni bir örnek oluşturur |
Redactor
akış kullanan şifre korumalı bir belge için sınıf.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Yeni bir örnek oluşturur |
Redactor
akış ve ayarları kullanan şifre korumalı bir belge için sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [close()](#close--) | Kaynakları serbest bırakır. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Belgeye bir redaksiyon uygular. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Belgeye bir dizi redaksiyon uygular. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Belgeye bir redaksiyon politikası uygular. |
|
|  | [save()](#save--) | Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Belgeyi bir dosyaya kaydeder. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Belgeyi bir akışa kaydeder. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Belgeyi bir akışa kaydeder. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Belgeyi bir akışa kaydeder, özel konumu dahil ederek. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Belirli sayfaların önizleme görüntülerini verilen bir görüntü formatında oluşturur. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Belge hakkında genel bilgileri alır - boyut, sayfa sayısı vb. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Yeni bir örnek oluşturur
Redactor
dosya yolu kullanan sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu |


Aşağıdaki örnek, bir belgeyi redaksiyon için nasıl açacağını gösterir.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Burada redaksiyonları gerçekleştirmek için belge örneğini kullanabiliriz
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Yeni bir örnek oluşturur
Redactor
yolunu kullanan şifre korumalı bir belge için sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosya yolu. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Seçenekler, şifre dahil. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Yeni bir örnek oluşturur
Redactor
yolunu ve ayarlarını kullanan şifre korumalı bir belge için sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosya yolu. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Dosyaya bağlı seçenekler, şifre dahil. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Redaksiyon süreci için varsayılan ayarlar. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Yeni bir örnek oluşturur
Redactor
akış kullanan şifre korumalı bir belge için sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Seçenekler, şifre dahil. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Yeni bir örnek oluşturur
Redactor
akış ve ayarları kullanan şifre korumalı bir belge için sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Seçenekler, şifre dahil. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Redaksiyon süreci için varsayılan ayarlar. |
|

### close() {#close--}
```
public final void close()
```


Kaynakları serbest bırakır.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Belgeye bir redaksiyon uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Uygulanacak Redaction örneği |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Belgeye bir dizi redaksiyon uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Uygulanacak redaksiyonların bir dizisi |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Belgeye bir redaksiyon politikası uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redaksiyon politikası |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Redakte edilmiş belgenin yolu

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Belgeyi bir dosyaya kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Sonek eklemek veya rasterleştirmek için seçenekler |
|

**Returns:**
java.lang.String - Redakte edilmiş belgenin yolu

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Belgeyi bir akışa kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.OutputStream | Hedef akış |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Belgeyi bir akışa kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.OutputStream | Hedef akış |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Kaydetme seçenekleri |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Belgeyi bir akışa kaydeder, özel konumu dahil ederek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.OutputStream | Hedef akış |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Rasterleştirip rasterleştirmemek ve rasterleştirme için sayfaları belirtmek için seçenekler |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Belirli sayfaların önizleme görüntülerini verilen bir görüntü formatında oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Görüntü özellikleri ve sayfa aralığı ayarları |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Belge hakkında genel bilgileri alır - boyut, sayfa sayısı vb.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

