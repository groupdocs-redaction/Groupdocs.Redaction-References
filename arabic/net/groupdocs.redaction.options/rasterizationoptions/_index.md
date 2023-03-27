---
title: RasterizationOptions
second_title: GroupDocs.Redaction لمرجع .NET API
description: يوفر خيارات لتحويل الملفات إلى PDF .
type: docs
weight: 350
url: /ar/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

يوفر خيارات لتحويل الملفات إلى PDF .

```csharp
public class RasterizationOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | تهيئة مثيل جديد . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | الحصول على أو تحديد مستوى توافق PDF . |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت جميع الصفحات في المستند بحاجة إلى التحويل إلى صور ووضعها في ملف PDF واحد. يتم تعيين TRUE افتراضيًا على FALSE لتجنب التنقيط. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | يحصل على مؤشر ، ويكون صحيحًا إذا تم تعيين خيارات التنقيط المتقدمة. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | الحصول على أو تحديد عدد الصفحات المطلوب تحويلها إلى PDF . |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | الحصول على أو تحديد فهرس الصفحة الأولى (المستندة إلى 0) لتحويلها إلى PDF . |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | يمكنك استخدام هذه الطريقة لتسجيل خيار تنقيط متقدم للتطبيق. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | يمكنك استخدام هذه الطريقة لتسجيل خيار تنقيط متقدم للتطبيق. |

### ملاحظات

**يتعلم أكثر**

* مزيد من التفاصيل حول حفظ المستند كملف PDF نقطي: [حفظ في ملف PDF نقطي](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* مزيد من التفاصيل حول خيارات التنقيط: [حدد صفحات معينة لملف PDF النقطي](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### أمثلة

يوضح المثال التالي كيفية تعيين الخيارات لعملية التنقيط.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // قم بتنقيح البيانات الحساسة على الشريحة الأولى 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

يوضح المثال التالي كيفية تطبيق خيارات التنقيط المتقدمة بالإعدادات الافتراضية.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند بالخيارات الافتراضية (تحويل الصفحات إلى صور ، حفظ كملف PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

يوضح المثال التالي كيفية تطبيق خيار التنقيط المتقدم للحد مع الإعدادات المخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند بحدود مخصصة
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

يوضح المثال التالي كيفية تطبيق خيار التحويل النقطي المتقدم للضوضاء مع الإعدادات المخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند بالرقم المخصص وحجم تأثيرات الضوضاء
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

يوضح المثال التالي كيفية تطبيق خيار إمالة التنقيط المتقدم بإعدادات مخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند بتأثير الإمالة المخصص
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### أنظر أيضا

* مساحة الاسم [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
