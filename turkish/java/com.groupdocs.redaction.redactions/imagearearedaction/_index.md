---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir görüntü belgesinin verilen alanına renkli dikdörtgen yerleştiren bir kırpmayı temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Bir görüntü belgesinin verilen alanına renkli dikdörtgen yerleştiren bir kırpmayı temsil eder.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Belirli bir alan boyutunu redakte etmek için ImageAreaRedaction sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOptions()](#getOptions--) | Alır |
RegionReplacementOptions
renk ve alan parametreleri içeren seçenekler.
|
|  | [getTopLeft()](#getTopLeft--) | Kaldırılacak alanın sol üst konumunu alır |
|
|  | [getDescription()](#getDescription--) | Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Redaksiyonu verilen format örneğine uygular. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Belirli bir alan boyutunu redakte etmek için ImageAreaRedaction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Sol üst alan koordinatları |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Alan boyutu ve rengi |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Alır
RegionReplacementOptions
renk ve alan parametreleri içeren seçenekler.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Kaldırılacak alanın sol üst konumunu alır


**Returns:**
java.awt.Point - Kaldırılacak alanın sol üst konumu

### getDescription() {#getDescription--}
```
public String getDescription()
```


Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür.


**Returns:**
java.lang.String - Redaksiyon adı ve parametrelerini içeren metin.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Redaksiyonu verilen format örneğine uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Redaksiyon uygulamak için bir belge örneği |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

