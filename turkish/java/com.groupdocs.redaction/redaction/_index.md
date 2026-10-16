---
title: "Redaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Tüm redaksiyon türleri için temel soyut sınıfı temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Tüm redaksiyon türleri için temel soyut sınıfı temsil eder.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDescription()](#getDescription--) | Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Redaksiyonu verilen format örneğine uygular. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Redaksiyonu ve parametrelerini tanımlayan bir dize döndürür.


**Returns:**
java.lang.String - Redaksiyon adı ve parametrelerini içeren metin.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Redaksiyonu verilen format örneğine uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Redaksiyon uygulamak için bir belge örneği |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

