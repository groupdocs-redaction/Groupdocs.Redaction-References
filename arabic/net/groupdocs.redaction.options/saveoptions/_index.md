---
title: SaveOptions
second_title: GroupDocs.Redaction لمرجع .NET API
description: يوفر خيارات لتغيير اسم ملف الإخراج و / أو تحويل المستند إلى ملف PDF مستند إلى الصور تنقيط.
type: docs
weight: 380
url: /ar/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

يوفر خيارات لتغيير اسم ملف الإخراج و / أو تحويل المستند إلى ملف PDF مستند إلى الصور (تنقيط).

```csharp
public class SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | يقوم بتهيئة مثيل جديد بالإعدادات الافتراضية: تنقيط إلى PDF - خطأ ، أضف لاحقة - خطأ. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | تهيئة مثيل جديد بمعلمات معينة. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان اسم الملف بحاجة إلى التغيير قبل الحفظ. خطأ افتراضيًا. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | الحصول على إعدادات التنقيط . |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند بحاجة إلى التحويل إلى صور ووضعها في ملف PDF واحد. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | الحصول على أو تعيين لاحقة مخصصة لاسم ملف الإخراج. إذا لم يتم تحديده ، فإن[`SaveSuffix`](./savesuffix) سيتم استخدام ثابت. |

## مجالات

| اسم | وصف |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | يمثل قيمة اللاحقة الافتراضية ، وهي "منقحة" . |

### ملاحظات

**يتعلم أكثر**

* [احفظ مع الخيارات الافتراضية](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [حفظ في ملف PDF نقطي](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [حدد صفحات معينة لملف PDF النقطي](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [احفظ في الشكل الأصلي](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [احفظ الكتابة فوق الملف الأصلي](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [حفظ في الدفق](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### أمثلة

يوضح المثال التالي كيفية حفظ مستند باستخدام SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // يتم وضع تنقيح المستند هنا
       // ...
    
       // احفظ المستند بالخيارات الافتراضية (تحويل الصفحات إلى صور ، حفظ كملف PDF)
       redactor.Save();
    
       // احفظ المستند بالتنسيق الأصلي للكتابة فوق الملف الأصلي
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // احفظ المستند في ملف "* _Redacted. *" بالتنسيق الأصلي
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // احفظ المستند إلى "* _AnyText. *" (مثل الطابع الزمني بدلاً من "AnyText") في اسم الملف الخاص به بدون التنقيط
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### أنظر أيضا

* مساحة الاسم [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
