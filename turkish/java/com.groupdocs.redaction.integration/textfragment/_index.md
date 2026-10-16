---
title: "TextFragment"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "OCR motoru tarafından çıkarılan tanınmış metin, kelime, sembol vb. bir bölümünü temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

OCR motoru tarafından çıkarılan tanınan metnin (kelime, sembol vb.) bir bölümünü temsil eder.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Tanınmış metin parçacığının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getText()](#getText--) | Tanınmış metin parçacığının metinsel içeriğini alır. |
|
|  | [getRectangle()](#getRectangle--) | Tanınmış metin parçacığının sınırlayıcı dikdörtgenini alır. |
|
|  | [toString()](#toString--) | Tanınmış metin parçacığının metinsel içeriğini döndürür. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Tanınmış metin parçacığının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | text | java.lang.String | tanınmış metin parçacığının metinsel içeriği |
|
|  | rectangle | java.awt.Rectangle | tanınmış metin parçacığının sınırlayıcı dikdörtgeni |
|

### getText() {#getText--}
```
public final String getText()
```


Tanınmış metin parçacığının metinsel içeriğini alır.


**Returns:**
java.lang.String - Tanınmış metin parçacığının metinsel içeriği.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Tanınmış metin parçacığının sınırlayıcı dikdörtgenini alır.


**Returns:**
java.awt.Rectangle - Tanınmış metin parçacığının sınırlayıcı dikdörtgeni.

### toString() {#toString--}
```
public String toString()
```


Tanınmış metin parçacığının metinsel içeriğini döndürür.


**Returns:**
java.lang.String - tanınmış metin parçacığının metinsel içeriği

