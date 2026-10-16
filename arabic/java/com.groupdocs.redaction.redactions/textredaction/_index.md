---
title: "TextRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل فئة أساسية مجردة لإزالة نصوص المستند."
type: docs
weight: 32
url: /ar/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

يمثل فئة أساسية مجردة لإزالة نصوص المستند.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | يحصل على |
ReplacementOptions
مثيل، يحدد نوع استبدال النص.
|
|  | [getOcrConnector()](#getOcrConnector--) | يحصل على |
IOcrConnector
تنفيذ، مطلوب لاستخراج النص من المحتوى الرسومي.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | يضبط |
IOcrConnector
تنفيذ، مطلوب لاستخراج النص من المحتوى الرسومي.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


يحصل على
ReplacementOptions
مثيل، يحدد نوع استبدال النص.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


يحصل على
IOcrConnector
تنفيذ، مطلوب لاستخراج النص من المحتوى الرسومي.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


يضبط
IOcrConnector
تنفيذ، مطلوب لاستخراج النص من المحتوى الرسومي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | تنفيذ IOcrConnector، مطلوب لاستخراج النص من المحتوى الرسومي. |
|

