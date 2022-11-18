---
title: Redactor
second_title: GroupDocs.Redaction لمرجع .NET API
description: يمثل فئة رئيسية تتحكم في عملية تنقيح المستندات  مما يسمح بفتح المستندات وتنقيحها وحفظها.
type: docs
weight: 650
url: /ar/net/groupdocs.redaction/redactor/
---
## Redactor class

يمثل فئة رئيسية تتحكم في عملية تنقيح المستندات ، مما يسمح بفتح المستندات وتنقيحها وحفظها.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة باستخدام الدفق. |
| [Redactor](redactor#constructor_3)(string) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة باستخدام مسار الملف. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة لمستند محمي بكلمة مرور باستخدام الدفق. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة لمستند محمي بكلمة مرور باستخدام مساره. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة لمستند محمي بكلمة مرور باستخدام الدفق والإعدادات. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | يقوم بتهيئة مثيل جديد من[`Redactor`](../redactor) فئة لمستند محمي بكلمة مرور باستخدام مساره وإعداداته. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | لتطبيق تنقيح على المستند. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | لتطبيق سياسة التنقيح على المستند. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | يطبق مجموعة من التنقيحات على المستند. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | إصدارات الموارد . |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | يولد صور معاينة لصفحات معينة بتنسيق صورة معين. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | الحصول على المعلومات العامة حول المستند - الحجم وعدد الصفحات وما إلى ذلك. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | يحفظ المستند في ملف بالخيارات التالية: AddSuffix = true ، RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | يحفظ المستند في ملف . |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | يحفظ المستند في دفق ، بما في ذلك الموقع المخصص. |

### ملاحظات

**يتعلم أكثر**

* مزيد من التفاصيل حول تطبيق التنقيحات: [أساسيات التنقيح](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* مواضيع تنقيح أكثر تقدمًا: [الاستخدام المتقدم](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### أمثلة

يوضح المثال التالي تطبيق تنقيح واحد على المستند.

يوضح المثال التالي تطبيق قائمة التنقيحات على المستند.

يوضح المثال التالي كيفية تطبيق سياسة التنقيح على جميع الملفات داخل مجلد وارد معين ، وحفظها في أحد المجلدات الصادرة - للملفات التي تم تحديثها بنجاح والملفات الفاشلة.

يوضح المثال التالي كيفية فتح مستندات محمية بكلمة مرور باستخدام LoadOptions.

يوضح المثال التالي كيفية حفظ مستند باستخدام SaveOptions.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... تنقيحات أخرى
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // خطأ ، إذا فشل تنقيح واحد على الأقل
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // هنا يمكننا استخدام مثيل المستند لإجراء التنقيحات
}
```

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

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* مساحة الاسم [GroupDocs.Redaction](../../groupdocs.redaction)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
