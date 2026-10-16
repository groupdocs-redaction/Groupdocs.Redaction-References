---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل النتائج لقائمة من عمليات الإخفاء التي تم تمريرها إلى طريقة Apply في فئة Redactor."
type: docs
weight: 17
url: /ar/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

يمثل النتائج لقائمة من عمليات الإخفاء، التي تم تمريرها إلى طريقة Apply() في
Redactor
الفئة.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | ينشئ مثيلاً جديداً من فئة RedactorChangeLog. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getStatus()](#getStatus--) | يحصل على الحالة النهائية لجميع عمليات الإخفاء المطبقة. |
|
|  | [getRedactionLog()](#getRedactionLog--) | يحصل على قائمة الـ |
RedactorLogEntry
instances.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


ينشئ مثيلاً جديداً من فئة RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


يحصل على الحالة النهائية لجميع عمليات الإخفاء المطبقة.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


يحصل على قائمة الـ
RedactorLogEntry
instances.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - قائمة كائنات RedactorLogEntry.

