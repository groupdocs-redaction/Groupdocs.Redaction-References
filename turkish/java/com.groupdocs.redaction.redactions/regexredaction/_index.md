---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder."
type: docs
weight: 28
url: /tr/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction sınıfının yeni bir örneğini başlatır. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Eşleşecek düzenli ifadeyi alır. |
|
|  | [getDescription()](#getDescription--) | Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Redaksiyonu verilen format örneğine uygular. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


RegexRedaction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Arama ve değiştirme için düzenli ifade |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Değiştirme seçenekleri (metinsel, renk) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


RegexRedaction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Arama ve değiştirme için düzenli ifade |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Değiştirme seçenekleri (metinsel, renk) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Eşleşecek düzenli ifadeyi alır.


**Returns:**
java.util.regex.Pattern - Eşleşecek düzenli ifade.

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

