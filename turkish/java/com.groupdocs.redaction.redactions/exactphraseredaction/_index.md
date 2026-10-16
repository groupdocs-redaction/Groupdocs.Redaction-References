---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belirli bir metin redaksiyonunu temsil eder ve belgelerin metnindeki tam ifadeyi varsayılan olarak büyük/küçük harfe duyarsız şekilde değiştirir."
type: docs
weight: 17
url: /tr/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Belgenin metnindeki tam ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız şekilde değiştiren bir metin kırpmasını temsil eder.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Aşağıdaki örnek, büyük/küçük harfe duyarlı ifade arama ve değiştirme işlemini göstermektedir.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Varsayılan olarak, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | ExactPhraseRedaction sınıfının yeni bir örneğini büyük/küçük harfe duyarsız modda başlatır. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | ExactPhraseRedaction sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Aranacak ve değiştirilecek dizeyi alır. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren bir değeri alır. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Bu metnin sağdan sola olup olmadığını gösteren bir değeri alır, varsayılan olarak false. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Bu metnin sağdan sola olup olmadığını gösteren bir değeri ayarlar, varsayılan olarak false. |
|
|  | [getDescription()](#getDescription--) | Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Redaksiyonu verilen format örneğine uygular. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


ExactPhraseRedaction sınıfının yeni bir örneğini büyük/küçük harfe duyarsız modda başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Aranacak ve değiştirilecek dize |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Değiştirme seçenekleri (metinsel, renk) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


ExactPhraseRedaction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Aranacak ve değiştirilecek dize |
|
|  | isCaseSensitive | boolean | Büyük/küçük harfe duyarlı arama gerekiyorsa true |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Değiştirme seçenekleri (metinsel, renk) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Aranacak ve değiştirilecek dizeyi alır.


**Returns:**
java.lang.String - Aranacak ve değiştirilecek dize.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren bir değeri alır.


**Returns:**
boolean - Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren bir değer.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Bu metnin sağdan sola olup olmadığını gösteren bir değeri alır, varsayılan olarak false.


**Returns:**
boolean - Bu metnin sağdan sola olup olmadığını gösteren bir değer, varsayılan olarak false.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Bu metnin sağdan sola olup olmadığını gösteren bir değeri ayarlar, varsayılan olarak false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Bu metnin sağdan sola olup olmadığını gösteren bir değer, varsayılan olarak false. |
|

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

