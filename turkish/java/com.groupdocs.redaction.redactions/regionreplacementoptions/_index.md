---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Görüntü bölgesi değiştirme için renk ve alan parametrelerini temsil eder."
type: docs
weight: 29
url: /tr/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Görüntü bölgesi değiştirme için renk ve alan parametrelerini temsil eder. Bkz
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | RegionReplacementOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Boyutu verilen metne uyan RegionReplacementOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Kırpılmış alanı doldurmak için rengi alır. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Kırpılmış alanı doldurmak için rengi ayarlar. |
|
|  | [getSize()](#getSize--) | Genişlik ve yükseklik ile dikdörtgeni alır. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Genişlik ve yükseklik ile dikdörtgeni ayarlar. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


RegionReplacementOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Alanı doldurmak için renk |
|
|  | boyut | java.awt.Dimension | Doldurulmuş alan boyutu |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Boyutu verilen metne uyan RegionReplacementOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Alanı doldurmak için renk |
|
|  | font | java.awt.Font | Beklenen metin yazı tipi |
|
|  | expectedText | java.lang.String | Beklenen metin |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Kırpılmış alanı doldurmak için rengi alır.


**Returns:**
java.awt.Color - Kırpılmış alanı doldurmak için renk.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Kırpılmış alanı doldurmak için rengi ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.awt.Color | Kırpılmış alanı doldurmak için renk. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Genişlik ve yükseklik ile dikdörtgeni alır.


**Returns:**
java.awt.Dimension - Genişlik ve yükseklik ile dikdörtgen.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Genişlik ve yükseklik ile dikdörtgeni ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.awt.Dimension | Genişlik ve yükseklik ile dikdörtgen. |
|

