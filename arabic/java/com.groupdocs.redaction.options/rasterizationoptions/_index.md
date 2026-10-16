---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر خيارات لتحويل الملفات إلى PDF."
type: docs
weight: 12
url: /ar/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

يوفر خيارات لتحويل الملفات إلى PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | يقوم بإنشاء نسخة جديدة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | يحصل على قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
|
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة الأولى (بدءًا من الصفر) للتحويل إلى PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | يضبط فهرس الصفحة الأولى (بدءًا من الصفر) للتحويل إلى PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | يحصل على قيمة تشير إلى ما إذا تم تغيير خاصية PageIndex (تم ضبطها) بعد تهيئتها. |
|
|  | [getPageCount()](#getPageCount--) | يحصل على عدد الصفحات التي سيتم تحويلها إلى PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | يضبط عدد الصفحات التي سيتم تحويلها إلى PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | يحصل على قيمة تشير إلى ما إذا كانت خاصية PageCount قد تم تغييرها (تعيينها) بعد تهيئتها. |
|
|  | [getCompliance()](#getCompliance--) | يحصل على مستوى توافق PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | يضبط مستوى توافق PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | يحصل على مؤشر يكون صحيحًا إذا تم تعيين خيارات الترصيص المتقدمة. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | يمكنك استخدام هذه الطريقة لتسجيل خيار ترصيص متقدم لتطبيقه. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | يمكنك استخدام هذه الطريقة لتسجيل خيار ترصيص متقدم لتطبيقه. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


يقوم بإنشاء نسخة جديدة.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


يحصل على قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند تحتاج إلى تحويلها إلى صور ووضعها في ملف PDF واحد. TRUE بشكل افتراضي، يتم تعيينها إلى FALSE لتجنب الترصيص.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند تحتاج إلى تحويلها إلى صور ووضعها في ملف PDF واحد. TRUE بشكل افتراضي، يتم تعيينها إلى FALSE لتجنب الترصيص.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند تحتاج إلى تحويلها إلى صور ووضعها في ملف PDF واحد. TRUE بشكل افتراضي، يتم تعيينها إلى FALSE لتجنب الترصيص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند تحتاج إلى تحويلها إلى صور ووضعها في ملف PDF واحد. TRUE بشكل افتراضي، يتم تعيينها إلى FALSE لتجنب الترصيص. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


يحصل على فهرس الصفحة الأولى (بدءًا من الصفر) للتحويل إلى PDF.


**Returns:**
int - فهرس الصفحة الأولى (بدءًا من 0) للتحويل إلى PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


يضبط فهرس الصفحة الأولى (بدءًا من الصفر) للتحويل إلى PDF.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | فهرس الصفحة الأولى (بدءًا من 0) للتحويل إلى PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


يحصل على قيمة تشير إلى ما إذا تم تغيير خاصية PageIndex (تم ضبطها) بعد تهيئتها.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت خاصية PageIndex قد تم تغييرها (تعيينها) بعد تهيئتها.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


يحصل على عدد الصفحات التي سيتم تحويلها إلى PDF.


**Returns:**
int - عدد الصفحات التي سيتم تحويلها إلى PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


يضبط عدد الصفحات التي سيتم تحويلها إلى PDF.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | عدد الصفحات التي سيتم تحويلها إلى PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


يحصل على قيمة تشير إلى ما إذا كانت خاصية PageCount قد تم تغييرها (تعيينها) بعد تهيئتها.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت خاصية PageCount قد تم تغييرها (تعيينها) بعد تهيئتها.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


يحصل على مستوى توافق PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


يضبط مستوى توافق PDF.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | مستوى توافق PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


يحصل على مؤشر يكون صحيحًا إذا تم تعيين خيارات الترصيص المتقدمة.


**Returns:**
boolean - مؤشر يكون صحيحًا إذا تم تعيين خيارات الترصيص المتقدمة.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


يمكنك استخدام هذه الطريقة لتسجيل خيار ترصيص متقدم لتطبيقه.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | يوفر معلومات حول نوع التأثير المحدد (تدرج الرمادي، حد، إلخ). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


يمكنك استخدام هذه الطريقة لتسجيل خيار ترصيص متقدم لتطبيقه.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | يوفر معلومات حول نوع التأثير المحدد (تدرج الرمادي، حد، إلخ). |
|
|  | معلمات | java.util.HashMap<java.lang.String,java.lang.String> | معلمات للتأثير المحدد، مثل زاوية الدوران |
|

