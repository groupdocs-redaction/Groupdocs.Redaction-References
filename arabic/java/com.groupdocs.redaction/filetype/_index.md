---
title: "FileType"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل نوع ملف."
type: docs
weight: 11
url: /ar/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

يمثل نوع ملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات المدعومة من قبل GroupDocs.Redaction، واكتشاف نوع الملف حسب الامتداد، إلخ.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | يحصل على اسم نوع الملف، على سبيل المثال "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | يحصل على لاحقة اسم الملف (بما في ذلك النقطة ".")، على سبيل المثال ".doc". |
|
|  | [getUnknown()](#getUnknown--) | يمثل نوع ملف غير معروف. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | صورة JPEG (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | صورة JPEG (.jpeg) |
|
|  | [getPNG()](#getPNG--) | صورة شبكة محمولة (.png) |
|
|  | [getGIF()](#getGIF--) | ملف تنسيق تبادل رسومي (.gif) |
|
|  | [getBMP()](#getBMP--) | ملف صورة نقطية (.bmp) |
|
|  | [getJP2()](#getJP2--) | ملف صورة JPEG 2000 الأساسي (.jp2) |
|
|  | [getHTM()](#getHTM--) | ملف لغة ترميز النص الفائق (.htm) |
|
|  | [getHTML()](#getHTML--) | ملف لغة ترميز النص الفائق (.html) |
|
|  | [getPDF()](#getPDF--) | ملف تنسيق المستند المحمول (.pdf) |
|
|  | [getPPT()](#getPPT--) | عرض PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | عرض PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | عرض OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | قالب عرض PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | قالب عرض PowerPoint Open XML مع تمكين الماكرو (.potm) |
|
|  | [getOTP()](#getOTP--) | قالب عرض OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | جدول بيانات Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | جدول بيانات Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | جدول بيانات Excel Open XML مع تمكين الماكرو (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | جدول بيانات Excel الثنائي (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | قالب جدول بيانات Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | قالب جدول بيانات Excel Open XML مع تمكين الماكرو (.xltm) |
|
|  | [getXLT()](#getXLT--) | قالب Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | ملف قيم مفصولة بفواصل (.csv) |
|
|  | [getTSV()](#getTSV--) | ملف قيم مفصولة بعلامات جدولة (.tsv) |
|
|  | [getTAB()](#getTAB--) | ملف قيم مفصولة بعلامات جدولة (.tab) |
|
|  | [getODS()](#getODS--) | جدول بيانات OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | قالب جدول بيانات OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | جدول بيانات Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | ملف توثيق Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | مستند Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | مستند Microsoft Word Open XML (.docx) |
|
|  | [getDOCM()](#getDOCM--) | مستند Word Open XML مع تمكين الماكرو (.docm) |
|
|  | [getDOT()](#getDOT--) | قالب مستند Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | قالب مستند Word Open XML (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | قالب مستند Word Open XML مع تمكين الماكرو (.dotm) |
|
|  | [getRTF()](#getRTF--) | ملف تنسيق النص الغني (.rtf) |
|
|  | [getTXT()](#getTXT--) | ملف نص عادي (.txt) |
|
|  | [getODT()](#getODT--) | مستند نص OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | قالب مستند OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | يربط امتداد الملف بنوع الملف. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | يسترجع أنواع الملفات المدعومة |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | يحدد ما إذا كان الحالي |
FileType
هو نفسه كما هو محدد
FileType
كائن.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان الحالي |
FileType
هو نفسه كائن محدد.
|
|  | [hashCode()](#hashCode--) | يعيد رمز التجزئة للعنصر الحالي |
FileType
كائن.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | يحدد ما إذا كان اثنان |
FileType
الكائنات هي نفسها.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | يحدد ما إذا كان اثنان |
FileType
الكائنات ليست هي نفسها.
|
|  | [toString()](#toString--) | يعيد سلسلة تمثل الكائن الحالي. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


يحصل على اسم نوع الملف، على سبيل المثال "Microsoft Word Document".


**Returns:**
java.lang.String - اسم نوع الملف، على سبيل المثال "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


يحصل على لاحقة اسم الملف (بما في ذلك النقطة ".")، على سبيل المثال ".doc".


**Returns:**
java.lang.String - لاحقة اسم الملف (بما في ذلك النقطة "."), على سبيل المثال ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


يمثل نوع ملف غير معروف.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Tagged Image File (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Tagged Image File Format (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


صورة JPEG (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


صورة JPEG (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


صورة شبكة محمولة (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


ملف تنسيق تبادل رسومي (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


ملف صورة نقطية (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


ملف صورة JPEG 2000 الأساسي (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


ملف لغة ترميز النص الفائق (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


ملف لغة ترميز النص الفائق (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


ملف تنسيق المستند المحمول (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


عرض PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


عرض PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


عرض OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


قالب عرض PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


قالب عرض PowerPoint Open XML مع تمكين الماكرو (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


قالب عرض OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


جدول بيانات Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


جدول بيانات Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


جدول بيانات Excel Open XML مع تمكين الماكرو (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


جدول بيانات Excel الثنائي (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


قالب جدول بيانات Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


قالب جدول بيانات Excel Open XML مع تمكين الماكرو (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


قالب Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


ملف قيم مفصولة بفواصل (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


ملف قيم مفصولة بعلامات جدولة (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


ملف قيم مفصولة بعلامات جدولة (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


جدول بيانات OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


قالب جدول بيانات OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


جدول بيانات Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


ملف توثيق Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


مستند Microsoft Word (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


مستند Microsoft Word Open XML (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


مستند Word Open XML مع تمكين الماكرو (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


قالب مستند Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


قالب مستند Word Open XML (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


قالب مستند Word Open XML مع تمكين الماكرو (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


ملف تنسيق النص الغني (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


ملف نص عادي (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


مستند نص OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


قالب مستند OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


يربط امتداد الملف بنوع الملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الامتداد | java.lang.String | امتداد الملف (بما في ذلك النقطة "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


يسترجع أنواع الملفات المدعومة


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - يُرجِع تسلسل أنواع الملفات المدعومة

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


يحدد ما إذا كان الحالي
FileType
هو نفسه كما هو محدد
FileType
كائن.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | الكائن للمقارنة مع كائن  FileType  الحالي. |
|

**Returns:**
منطقي - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the current 
FileType
 is the same as specified object.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object.
 |

**Returns:**
boolean - ```
true
```

إذا

```
obj
```

المعامل هو  FileType  وهو نفسه ككائن  FileType  الحالي؛ وإلا،

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد رمز التجزئة للعنصر الحالي
FileType
كائن.


**Returns:**
int - رمز تجزئة لكائن  FileType  الحالي.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


يحدد ما إذا كان اثنان
FileType
الكائنات هي نفسها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | كائن  FileType  الأيسر. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | كائن  FileType  الأيمن. |
|

**Returns:**
منطقي - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### op_Inequality(FileType left, FileType right) {#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Inequality(FileType left, FileType right)
```


Determines whether two 
FileType
 objects are not the same.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object.
 |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object.
 |

**Returns:**
boolean - ```
true
```

إذا كان كائـنـا  FileType  غير متساويين؛ وإلا،

```
false
```


### toString() {#toString--}
```
public String toString()
```


يعيد سلسلة تمثل الكائن الحالي.


**Returns:**
java.lang.String - سلسلة تمثل الكائن الحالي.

