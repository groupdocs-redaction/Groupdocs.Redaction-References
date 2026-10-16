---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يوفر خيارات لتعيين المتطلبات ومندوبين التدفق لتوليد المعاينة."
type: docs
weight: 11
url: /ar/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

يوفر خيارات لتعيين المتطلبات ومندوبين التدفق لتوليد المعاينة.

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | يقوم بإنشاء نسخة جديدة من الفئة PreviewOptions، مما يؤدي إلى إغلاق تدفق الإخراج. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | يقوم بإنشاء نسخة جديدة من الفئة PreviewOptions، مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام الإضافي. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getWidth()](#getWidth--) | يحصل أو يضبط عرض معاينة الصفحة. |
|
|  | [setWidth(int value)](#setWidth-int-) | يحصل أو يضبط عرض معاينة الصفحة. |
|
|  | [getHeight()](#getHeight--) | يحصل أو يضبط ارتفاع معاينة الصفحة. |
|
|  | [setHeight(int value)](#setHeight-int-) | يحصل أو يضبط ارتفاع معاينة الصفحة. |
|
|  | [getPageNumbers()](#getPageNumbers--) | يحصل أو يضبط مصفوفة أرقام الصفحات لتوليد المعاينة. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | يحصل أو يضبط مصفوفة أرقام الصفحات لتوليد المعاينة. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | يحصل أو يضبط تنسيق صورة المعاينة. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | يحصل أو يضبط تنسيق صورة المعاينة. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | يحصل أو يضبط نسخة من مفوض إنشاء تدفق الصفحة. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | يحصل أو يضبط نسخة من مفوض إنشاء تدفق الصفحة. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | يحصل أو يضبط نسخة من مفوض إكمال معاينة الصفحة. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | يحصل أو يضبط نسخة من مفوض إكمال معاينة الصفحة. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


يقوم بإنشاء نسخة جديدة من الفئة PreviewOptions، مما يؤدي إلى إغلاق تدفق الإخراج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | ينشئ تدفقًا لمعاينة صفحة محددة |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


يقوم بإنشاء نسخة جديدة من الفئة PreviewOptions، مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام الإضافي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | ينشئ تدفقًا لمعاينة صفحة محددة |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | يُخطر بأن توليد معاينة الصفحة انتهى ويحصل على تدفق الإخراج |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


يحصل أو يضبط عرض معاينة الصفحة.


**Returns:**
int - عرض معاينة الصفحة.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


يحصل أو يضبط عرض معاينة الصفحة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | عرض معاينة الصفحة. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


يحصل أو يضبط ارتفاع معاينة الصفحة.


**Returns:**
int - ارتفاع معاينة الصفحة.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


يحصل أو يضبط ارتفاع معاينة الصفحة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | ارتفاع معاينة الصفحة. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


يحصل أو يضبط مصفوفة أرقام الصفحات لتوليد المعاينة.


**Returns:**
int[] - مصفوفة أرقام الصفحات لتوليد المعاينة.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


يحصل أو يضبط مصفوفة أرقام الصفحات لتوليد المعاينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int[] | مصفوفة أرقام الصفحات لتوليد المعاينة. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


يحصل أو يضبط تنسيق صورة المعاينة.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


يحصل أو يضبط تنسيق صورة المعاينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | تنسيق صورة المعاينة. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


يحصل أو يضبط نسخة من مفوض إنشاء تدفق الصفحة.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


يحصل أو يضبط نسخة من مفوض إنشاء تدفق الصفحة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | نسخة من مفوض إنشاء تدفق الصفحة. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


يحصل أو يضبط نسخة من مفوض إكمال معاينة الصفحة.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


يحصل أو يضبط نسخة من مفوض إكمال معاينة الصفحة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | نسخة من مفوض إكمال معاينة الصفحة. |
|

