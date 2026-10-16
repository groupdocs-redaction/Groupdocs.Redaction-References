---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir belgenin sayfası içinde bir alanı ayarlayarak redaksiyon uygulayan redaksiyon filtresini temsil eder."
type: docs
weight: 22
url: /tr/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Redaksiyon filtresini temsil eder, bir belgenin sayfası içinde redaksiyon uygulanacak bir alanı ayarlar.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Belirli bir alanı redakte etmek için PageAreaFilter sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Bir sayfadaki dikdörtgeni (alanın sol üst konumu ve boyutu) alır. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Bu filtre alanının verilen dikdörtgenle kesişip kesişmediğini kontrol eder. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Belirli bir alanı redakte etmek için PageAreaFilter sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Sol üst alan koordinatları |
|
|  | boyut | java.awt.Dimension | Alan boyutu ve rengi |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Bir sayfadaki dikdörtgeni (alanın sol üst konumu ve boyutu) alır.


**Returns:**
java.awt.Rectangle - Bir sayfadaki dikdörtgen (alanın sol üst konumu ve boyutu).

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Bu filtre alanının verilen dikdörtgenle kesişip kesişmediğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Kontrol edilecek dikdörtgen |
|

**Returns:**
boolean - true, eğer bu filtre alanı kesişim içeriyorsa

