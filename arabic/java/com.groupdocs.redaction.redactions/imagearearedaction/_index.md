---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل تشويهًا يضع مستطيلًا ملونًا في المنطقة المحددة من مستند صورة."
type: docs
weight: 18
url: /ar/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

يمثل تشويهًا يضع مستطيلًا ملونًا في المنطقة المحددة من مستند صورة.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | ينشئ مثيلاً جديداً من الفئة ImageAreaRedaction لتعديل حجم منطقة محددة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getOptions()](#getOptions--) | يحصل على |
RegionReplacementOptions
خيارات مع معلمات اللون والمنطقة.
|
|  | [getTopLeft()](#getTopLeft--) | يحصل على موضع الزاوية العليا اليسرى للمنطقة التي سيتم إزالتها |
|
|  | [getDescription()](#getDescription--) | يرجع سلسلة نصية تصف الحذف ومعامِلاته. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


ينشئ مثيلاً جديداً من الفئة ImageAreaRedaction لتعديل حجم منطقة محددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | topLeft | java.awt.Point | إحداثيات المنطقة العلوية اليسرى |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | حجم المنطقة واللون |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


يحصل على
RegionReplacementOptions
خيارات مع معلمات اللون والمنطقة.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


يحصل على موضع الزاوية العليا اليسرى للمنطقة التي سيتم إزالتها


**Returns:**
java.awt.Point - موضع الزاوية العليا اليسرى للمنطقة التي سيتم إزالتها

### getDescription() {#getDescription--}
```
public String getDescription()
```


يرجع سلسلة نصية تصف الحذف ومعامِلاته.


**Returns:**
java.lang.String - نص يحتوي على اسم الحذف ومعامِلاته.

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

