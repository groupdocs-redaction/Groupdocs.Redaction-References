---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل فئة أساسية مجردة لإزالة بيانات تعريف المستند."
type: docs
weight: 20
url: /ar/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

يمثل فئة أساسية مجردة لإزالة بيانات تعريف المستند.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getFilter()](#getFilter--) | يحصل على الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company. |
|
|  | [setFilter(int value)](#setFilter-int-) | يضبط الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


يحصل على الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company.


**Returns:**
int - الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


يضبط الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | الفلتر الذي يُستخدم لاختيار كل البيانات الوصفية أو بعضها، على سبيل المثال Author أو Company. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


يطبق الحذف على نسخة تنسيق معينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | نسخة من مستند لتطبيق الحذف |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

