---
title: "RedactableImage"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Tüm raster görüntü redaksiyon işlemlerine bir arayüz sağlar."
type: docs
weight: 14
url: /tr/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Tüm raster görüntü redaksiyon işlemlerine bir arayüz sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Bir nesne kullanarak yeni bir örnek oluşturur, uygulayan |
IImageFormatInstance
arayüz.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Bir nesne kullanarak yeni bir örnek oluşturur, uygulayan |
IMultipleAreaRedactable
arayüz.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Gerçek görüntü içeriğine sahip bir akışı alır. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Aynı renk ile birden fazla görüntü alanını aynı anda karartır. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Belirtilen noktadaki alanı belirli renk ve boyutta bir dikdörtgenle değiştirir. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Bir nesne kullanarak yeni bir örnek oluşturur, uygulayan
IImageFormatInstance
arayüz.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | IImageFormatInstance arayüzünü uygulayan bir örnek |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Bir nesne kullanarak yeni bir örnek oluşturur, uygulayan
IMultipleAreaRedactable
arayüz.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | IMultipleAreaRedactable arabirimini uygulayan bir örnek |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Gerçek görüntü içeriğine sahip bir akışı alır.


**Returns:**
java.io.InputStream - Görüntü verilerini içeren akış

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Aynı renk ile birden fazla görüntü alanını aynı anda karartır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dikdörtgenler | java.awt.Rectangle[] | Dikdörtgen alanların bir dizisi |
|
|  | boxColor | java.awt.Color | Alanları doldurmak için renk |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Belirtilen noktadaki alanı belirli renk ve boyutta bir dikdörtgenle değiştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Doldurulmuş alanın sol üst köşe koordinatları |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Renk ve boyut ayarları |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

