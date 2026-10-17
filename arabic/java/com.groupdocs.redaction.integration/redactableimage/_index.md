---
title: "RedactableImage"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر واجهة لجميع عمليات تعديل الصور النقطية."
type: docs
weight: 14
url: /ar/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

يوفر واجهة لجميع عمليات تعديل الصور النقطية.

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | ينشئ مثيلاً جديدًا باستخدام كائن، يطبق |
IImageFormatInstance
الواجهة.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | ينشئ مثيلاً جديدًا باستخدام كائن، يطبق |
IMultipleAreaRedactable
الواجهة.
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | يسترجع تدفقًا يحتوي على محتوى الصورة الفعلي. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | يحجب عدة مناطق صورة مرة واحدة بنفس اللون. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | يستبدل المنطقة عند النقطة المحددة بمستطيل بلون وحجم محددين. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


ينشئ مثيلاً جديدًا باستخدام كائن، يطبق
IImageFormatInstance
الواجهة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | مثيل، يطبق واجهة IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


ينشئ مثيلاً جديدًا باستخدام كائن، يطبق
IMultipleAreaRedactable
الواجهة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | مثيل، يطبق واجهة IMMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


يسترجع تدفقًا يحتوي على محتوى الصورة الفعلي.


**Returns:**
java.io.InputStream - تدفق يحتوي على بيانات الصورة

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


يحجب عدة مناطق صورة مرة واحدة بنفس اللون.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مستطيلات | java.awt.Rectangle[] | مصفوفة من مناطق المستطيلات |
|
|  | boxColor | java.awt.Color | اللون لملء المناطق |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


يستبدل المنطقة عند النقطة المحددة بمستطيل بلون وحجم محددين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | topLeft | java.awt.Point | إحداثيات الزاوية العلوية اليسرى للمنطقة المملوءة |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | إعدادات اللون والحجم |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

