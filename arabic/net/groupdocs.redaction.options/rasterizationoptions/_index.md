---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction لـ .NET مرجع API"
description: "يوفر خيارات لتحويل الملفات إلى PDF."
type: docs
weight: 420
url: /ar/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

يوفر خيارات لتحويل الملفات إلى PDF.

```csharp
public class RasterizationOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | يُهيئ نسخة جديدة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | يحصل أو يعيّن مستوى التوافق مع PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | يحصل أو يعيّن قيمة تُشير إلى ما إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. TRUE افتراضيًا، اضبطه إلى FALSE لتجنب التحويل إلى نقطية. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | يحصل على مؤشر يكون true إذا تم تعيين خيارات التحويل إلى نقطية المتقدمة. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | يحصل أو يعيّن عدد الصفحات التي سيتم تحويلها إلى PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | يحصل أو يعيّن فهرس الصفحة الأولى (بدءًا من 0) لتحويلها إلى PDF. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | يمكنك استخدام هذه الطريقة لتسجيل خيار تحويل نقطي متقدم لتطبيقه. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | يمكنك استخدام هذه الطريقة لتسجيل خيار تحويل نقطي متقدم لتطبيقه. |

### ملاحظات

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### أمثلة

يوضح المثال التالي كيفية ضبط الخيارات لعملية التحويل إلى نقطية.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // إزالة البيانات الحساسة من الشريحة الأولى
    
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

يوضح المثال التالي كيفية تطبيق خيارات الترصيص المتقدمة بالإعدادات الافتراضية.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند باستخدام الخيارات الافتراضية (تحويل الصفحات إلى صور، حفظ كملف PDF)
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

يوضح المثال التالي كيفية تطبيق خيار الترصيص المتقدم للحدود بالإعدادات المخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند بحد مخصص
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

يوضح المثال التالي كيفية تطبيق خيار الترصيص المتقدم للضوضاء بالإعدادات المخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند مع العدد المخصص وحجم تأثيرات الضوضاء
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

المثال التالي يوضح كيفية تطبيق خيار التدوير المتقدم مع الإعدادات المخصصة.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // احفظ المستند مع تأثير الميل المخصص
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### انظر أيضًا

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
