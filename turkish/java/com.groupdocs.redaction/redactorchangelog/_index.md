---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Redactor sınıfının Apply yöntemine geçirilen bir redaksiyon listesi için sonuçları temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Apply() yöntemine geçirilen bir redaksiyon listesi için sonuçları temsil eder
Redactor
sınıf.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | RedactorChangeLog sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getStatus()](#getStatus--) | Uygulanan tüm redaksiyonların son durumunu alır. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Listesini alır |
RedactorLogEntry
örnekleri.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


RedactorChangeLog sınıfının yeni bir örneğini başlatır.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Uygulanan tüm redaksiyonların son durumunu alır.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Listesini alır
RedactorLogEntry
örnekleri.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - RedactorLogEntry  örneklerinin listesini.

