---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir görüntüden tanıma süreci sonucunda çıkarılan metni temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Tanıma sürecinin bir sonucu olarak bir görüntüden çıkarılan metni temsil eder.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Tanıyan satırların bir kümesini kullanarak sınıfın yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getText()](#getText--) | Yapılandırılmış metnin metinsel eşdeğerini alır. |
|
|  | [getLines()](#getLines--) | Belge içinde tanınan metin satırlarını, parçacıklarıyla birlikte alır. |
|
|  | [toString()](#toString--) | Yapılandırılmış metnin metinsel eşdeğerini alır. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Tanıyan satırların bir kümesini kullanarak sınıfın yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | tanınan satırların bir IEnumerable'i (ör. bir liste veya dizi) |
|

### getText() {#getText--}
```
public final String getText()
```


Yapılandırılmış metnin metinsel eşdeğerini alır.


**Returns:**
java.lang.String - Yapılandırılmış metnin metinsel eşdeğeri.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Belge içinde tanınan metin satırlarını, parçacıklarıyla birlikte alır.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Belge içinde tanınan metin satırları, parçacıklarıyla birlikte.

### toString() {#toString--}
```
public String toString()
```


Yapılandırılmış metnin metinsel eşdeğerini alır.


**Returns:**
java.lang.String - Tanınan metin

