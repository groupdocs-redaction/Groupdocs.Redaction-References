---
title: "الحذف"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل الفئة الأساسية المجردة لجميع أنواع التمويه."
type: docs
weight: 13
url: /ar/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

يمثل الفئة الأساسية المجردة لجميع أنواع التمويه.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getDescription()](#getDescription--) | يرجع سلسلة نصية تصف الحذف ومعامِلاته. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


يرجع سلسلة نصية تصف الحذف ومعامِلاته.


**Returns:**
java.lang.String - نص يحتوي على اسم الحذف ومعامِلاته.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


يطبق الحذف على نسخة تنسيق معينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | نسخة من مستند لتطبيق الحذف |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

