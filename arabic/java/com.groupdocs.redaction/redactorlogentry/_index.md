---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل نتائج تطبيق التمويه."
type: docs
weight: 18
url: /ar/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

يمثل نتائج تطبيق التمويه.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | يُهيئ مثالًا جديدًا من فئة RedactorLogEntry للحذف. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getResult()](#getResult--) | يحصل على النتيجة، التي تُرجع بواسطة |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | يحصل على المرجع إلى الإزالة وخياراتها. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


يُهيئ مثالًا جديدًا من فئة RedactorLogEntry للحذف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | المرجع إلى الإزالة |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | نتيجة الإزالة، تم الإبلاغ عنها بواسطة معالج الصيغة |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


يحصل على النتيجة، التي تُرجع بواسطة
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


يحصل على المرجع إلى الإزالة وخياراتها.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

