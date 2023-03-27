---
title: FileType
second_title: GroupDocs.Redaction لمرجع .NET API
description: يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات التي يدعمها GroupDocs.Redaction واكتشاف نوع الملف حسب الامتداد وما إلى ذلك.
type: docs
weight: 90
url: /ar/net/groupdocs.redaction/filetype/
---
## FileType class

يمثل نوع الملف. يوفر طرقًا للحصول على قائمة بجميع أنواع الملفات التي يدعمها GroupDocs.Redaction واكتشاف نوع الملف حسب الامتداد وما إلى ذلك.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | ملف صورة نقطية (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | ملف القيم المفصولة بفواصل (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | مستند Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | مستند ممكّن بماكرو مفتوح XML لـ Word (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | مستند Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | قالب مستند Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML - قالب مستند ممكّن بماكرو (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML Document Template (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | ملف تنسيق التبادل الرسومي (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | ملف لغة توصيف النص التشعبي (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | ملف لغة ترميز النص التشعبي (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 Core Image File (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | صورة JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | صورة JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | ملف التوثيق Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | جدول بيانات أرقام Apple (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument Presentation (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | جدول بيانات OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | مستند نصي OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | قالب جدول بيانات OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | قالب مستند OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Portable Document Format File (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | رسم الشبكة المحمولة (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | عرض PowerPoint تقديمي (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML Presentation (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | ملف بتنسيق Rich Text (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | ملف الصور الموسومة (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | تنسيق ملف الصورة الموسوم (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | ملف القيم المفصولة بعلامات جدولة (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | ملف نصي عادي (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | يمثل نوع ملف غير معروف. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | جدول بيانات Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | جدول بيانات Excel ثنائي (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel فتح جدول بيانات ممكّن بماكرو XML (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML Spreadsheet (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | يحصل على لاحقة اسم الملف (بما في ذلك النقطة ".") ، على سبيل المثال ".doc" . |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | الحصول على اسم نوع الملف ، على سبيل المثال "مستند Microsoft Word". |

## طُرق

| اسم | وصف |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | امتداد ملف الخرائط لنوع الملف. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | يحدد ما إذا كان التيار[`FileType`](../filetype) هو نفسه كما هو محدد[`FileType`](../filetype) الكائن . |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | يحدد ما إذا كان التيار[`FileType`](../filetype) هو نفس الكائن المحدد. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | إرجاع كود التجزئة الحالي[`FileType`](../filetype) الكائن . |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | إرجاع سلسلة تمثل الكائن الحالي. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | استرداد أنواع الملفات المدعومة |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | تحديد ما إذا كان اثنان[`FileType`](../filetype) الكائنات هي نفسها. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | تحديد ما إذا كان اثنان[`FileType`](../filetype) الكائنات ليست هي نفسها. |

### ملاحظات

**يتعلم أكثر**

* [تنسيقات المستندات المدعومة](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [احصل على تنسيقات الملفات المدعومة](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [احصل على معلومات الملف](https://docs.groupdocs.com/redaction/net/get-file-info/)

### أنظر أيضا

* مساحة الاسم [GroupDocs.Redaction](../../groupdocs.redaction)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
