---
title: "SaveOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر خيارات لتغيير اسم ملف الإخراج و/أو تحويل المستند إلى تمثيل نقطي PDF قائم على الصور."
type: docs
weight: 14
url: /ar/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

يوفر خيارات لتغيير اسم ملف الإخراج و/أو تحويل المستند إلى PDF قائم على الصور (التصوير النقطي).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | يُهيئ نسخة جديدة بالإعدادات الافتراضية: التحويل إلى PDF نقطيًا - false، إضافة لاحقة - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | يقوم بتهيئة نسخة جديدة مع المعلمات المعطاة. |
|
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | يمثل قيمة اللاحقة الافتراضية، والتي هي "Redacted". |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | يحصل على قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | يحصل على لاحقة مخصصة لاسم ملف الإخراج. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | يضبط لاحقة مخصصة لاسم ملف الإخراج. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | يحصل على قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
|
|  | [getRasterization()](#getRasterization--) | يحصل على إعدادات التحويل إلى نقطية. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | خيارات حفظ معالجة النصوص. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


يُهيئ نسخة جديدة بالإعدادات الافتراضية: التحويل إلى PDF نقطيًا - false، إضافة لاحقة - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


يقوم بتهيئة نسخة جديدة مع المعلمات المعطاة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | صحيح، إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد |
|
|  | suffix | java.lang.String | سيتم إضافة هذا النص إلى نهاية اسم الملف، إذا لم يكن فارغًا سيضبط أيضًا AddSuffix إلى true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


يمثل قيمة اللاحقة الافتراضية، والتي هي "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. القيمة الافتراضية هي false.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. القيمة الافتراضية هي false.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | قيمة تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. القيمة الافتراضية هي false. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


يحصل على لاحقة مخصصة لاسم ملف الإخراج. إذا لم يتم تحديدها، فإن
SaveSuffix
الثابت سيُستخدم.


**Returns:**
java.lang.String - لاحقة مخصصة لاسم ملف الإخراج. إذا لم يتم تحديدها، فإن الثابت  SaveSuffix  سيُستخدم.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


يضبط لاحقة مخصصة لاسم ملف الإخراج. إذا لم يتم تحديدها، فإن
SaveSuffix
الثابت سيُستخدم.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | لاحقة مخصصة لاسم ملف الإخراج. إذا لم يتم تحديدها، سيتم استخدام الثابت SaveSuffix. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد.


**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


يحصل على إعدادات التحويل إلى نقطية.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


خيارات حفظ معالجة النصوص.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
