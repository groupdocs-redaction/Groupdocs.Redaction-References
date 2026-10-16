---
title: "Redactor"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل الفئة الرئيسية التي تتحكم في عملية تشفير المستند وتسمح بفتح وتحرير وحفظ المستندات."
type: docs
weight: 16
url: /ar/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable، [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

يمثل الفئة الرئيسية التي تتحكم في عملية تمويه المستند، وتسمح بفتح، تمويه وحفظ المستندات.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة تستخدم مسار الملف.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة تستخدم تدفقًا.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة لمستند محمي بكلمة مرور تستخدم مساره.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة لمستند محمي بكلمة مرور تستخدم مساره والإعدادات.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة لمستند محمي بكلمة مرور يستخدم تدفقًا.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | يُنشئ مثيلاً جديدًا من |
Redactor
فئة لمستند محمي بكلمة مرور يستخدم تدفقًا والإعدادات.
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [close()](#close--) | يطلق الموارد. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | يطبق تشفيرًا على المستند. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | يطبق مجموعة من التشفيرات على المستند. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | يطبق سياسة تشفير على المستند. |
|
|  | [save()](#save--) | يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | يحفظ المستند إلى ملف. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | يحفظ المستند إلى تدفق. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | يحفظ المستند إلى تدفق. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | يحفظ المستند إلى تدفق، بما في ذلك الموقع المخصص. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | يحصل على المعلومات العامة حول المستند - الحجم، عدد الصفحات، إلخ. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


يُنشئ مثيلاً جديدًا من
Redactor
فئة تستخدم مسار الملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار الملف |


يوضح المثال التالي كيفية فتح مستند للتشفير.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// هنا يمكننا استخدام نسخة المستند لإجراء عمليات الحذف
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا من
Redactor
فئة لمستند محمي بكلمة مرور تستخدم مساره.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | الخيارات، بما في ذلك كلمة المرور. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


يُنشئ مثيلاً جديدًا من
Redactor
فئة لمستند محمي بكلمة مرور تستخدم مساره والإعدادات.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | الخيارات المعتمدة على الملف، بما في ذلك كلمة المرور. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | الإعدادات الافتراضية لعملية الحذف. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا من
Redactor
فئة لمستند محمي بكلمة مرور يستخدم تدفقًا.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | الخيارات، بما في ذلك كلمة المرور. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


يُنشئ مثيلاً جديدًا من
Redactor
فئة لمستند محمي بكلمة مرور يستخدم تدفقًا والإعدادات.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | الخيارات، بما في ذلك كلمة المرور. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | الإعدادات الافتراضية لعملية الحذف. |
|

### close() {#close--}
```
public final void close()
```


يطلق الموارد.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


يطبق تشفيرًا على المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | مثال من Redaction لتطبيقه |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


يطبق مجموعة من التشفيرات على المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | مصفوفة من عمليات الحذف لتطبيقها |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


يطبق سياسة تشفير على المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | سياسة الحذف |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - المسار إلى المستند المحذوف

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


يحفظ المستند إلى ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | خيارات لإضافة لاحقة أو تحويل إلى نقطية |
|

**Returns:**
java.lang.String - المسار إلى المستند المحذوف

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


يحفظ المستند إلى تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.OutputStream | دفق الهدف |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


يحفظ المستند إلى تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.OutputStream | دفق الهدف |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | خيارات الحفظ |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


يحفظ المستند إلى تدفق، بما في ذلك الموقع المخصص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.OutputStream | دفق الهدف |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | خيارات لتحويل إلى نقطية أو لا وتحديد الصفحات للتحويل إلى نقطية |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | إعدادات خصائص الصورة ونطاق الصفحات |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


يحصل على المعلومات العامة حول المستند - الحجم، عدد الصفحات، إلخ.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

