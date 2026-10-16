---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redaksiyon uygulamasının sonuçlarını temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Redaksiyon uygulamasının sonuçlarını temsil eder.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Redaction için RedactorLogEntry sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getResult()](#getResult--) | Sonucu alır, döndüren |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Redaction ve seçeneklerine referansı alır. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Redaction için RedactorLogEntry sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Redaction referansı |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Format işleyicisi tarafından raporlanan redaction sonucu |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Sonucu alır, döndüren
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Redaction ve seçeneklerine referansı alır.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

