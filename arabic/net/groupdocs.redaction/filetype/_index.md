---
title: "FileType"
second_title: "GroupDocs.Redaction لـ .NET مرجع API"
description: "يمثل نوع ملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات المدعومة من قبل GroupDocs.Redaction واكتشاف نوع الملف حسب الامتداد إلخ."
type: docs
weight: 90
url: /ar/net/groupdocs.redaction/filetype/
---
## FileType class

يمثل نوع ملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات المدعومة من قبل GroupDocs.Redaction، واكتشاف نوع الملف بناءً على الامتداد، إلخ.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | ملف صورة نقطية (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | ملف القيم المفصولة بفواصل (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | صورة DjVu (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | مستند Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | مستند Word Open XML مع تمكين الماكرو (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | مستند Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | قالب مستند Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | قالب مستند Word Open XML مع تمكين الماكرو (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | قالب مستند Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | ملف تنسيق تبادل الرسوميات (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | ملف لغة ترميز النص الفائق (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | ملف لغة ترميز النص الفائق (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | ملف صورة JPEG 2000 الأساسي (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | صورة JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | صورة JPEG (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | ملف سجل (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | ملف توثيق Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | جدول بيانات Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | عرض تقديمي OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | جدول بيانات OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | مستند نص OpenDocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | قالب عرض تقديمي OpenDocument (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | قالب جدول بيانات OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | قالب مستند OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | ملف تنسيق المستندات القابل للنقل (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | رسوميات شبكة محمولة (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | قالب عرض تقديمي ماكرو-مفعل PowerPoint Open XML (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | قالب عرض تقديمي PowerPoint Open XML (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | عرض شرائح PowerPoint (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | شريحة ماكرو-مفعل PowerPoint Open XML (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | عرض شرائح PowerPoint Open XML (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | عرض تقديمي PowerPoint (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | عرض تقديمي ماكرو-مفعل PowerPoint Open XML |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | عرض تقديمي PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | ملف تنسيق النص الغني (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | ملف قيم مفصولة بعلامات جدولة (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | ملف صورة معلم (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | تنسيق ملف صورة معلم (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | ملف قيم مفصولة بعلامات جدولة (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | ملف نص عادي (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | يمثل نوع ملف غير معروف. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | صورة WebP (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | جدول بيانات Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | جدول بيانات Excel الثنائي (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | جدول بيانات ماكرو-مفعل Excel Open XML (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | جدول بيانات Microsoft Excel Open XML (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | قالب Excel (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | قالب جدول بيانات ماكرو-مفعل Excel Open XML (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | قالب جدول بيانات Excel Open XML (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | يحصل على لاحقة اسم الملف (بما في ذلك النقطة "."), على سبيل المثال ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | يحصل على اسم نوع الملف، على سبيل المثال "Microsoft Word Document". |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | يقوم بربط امتداد الملف بنوع الملف. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | يحدد ما إذا كان [`FileType`](../filetype) الحالي هو نفسه ككائن [`FileType`](../filetype) المحدد. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | يحدد ما إذا كان [`FileType`](../filetype) الحالي هو نفسه كالكائن المحدد. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | يعيد رمز التجزئة (hash code) لكائن [`FileType`](../filetype) الحالي. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | يعيد سلسلة تمثل الكائن الحالي. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | يسترجع أنواع الملفات المدعومة |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | يحدد ما إذا كان كائني [`FileType`](../filetype) متطابقين. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | يحدد ما إذا كان كائني [`FileType`](../filetype) غير متطابقين. |

### ملاحظات

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### انظر أيضًا

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
