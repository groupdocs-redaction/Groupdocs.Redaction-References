---
title: "TextLine"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "OCR motoru tarafından bir görüntüden çıkarılan bir metin satırını temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

OCR motoru tarafından bir görüntüden çıkarılan bir metin satırını temsil eder.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | OCR motoru tarafından bir görüntüden çıkarılan bir metin satırının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFragments()](#getFragments--) | Satırda tanınan semboller ve kelimeler gibi metin parçacıklarının bir dizisini alır. |
|
|  | [toString()](#toString--) | Tanınan metin satırının metinsel içeriğini döndürür. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


OCR motoru tarafından bir görüntüden çıkarılan bir metin satırının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | metin parçacıklarının ilk kümesi |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Satırda tanınan semboller ve kelimeler gibi metin parçacıklarının bir dizisini alır.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Satırda tanınan, semboller ve kelimeler gibi metin parçacıklarından oluşan bir dizi.

### toString() {#toString--}
```
public String toString()
```


Tanınan metin satırının metinsel içeriğini döndürür.


**Returns:**
java.lang.String - Tanınan metin satırının metinsel içeriği

