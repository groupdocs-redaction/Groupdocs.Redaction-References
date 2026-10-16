---
title: "Redactor"
second_title: "GroupDocs.Redaction لـ .NET مرجع API"
description: "يمثل الفئة الرئيسية التي تتحكم في عملية حذف محتوى المستند، وتسمح بفتح، حذف، وحفظ المستندات."
type: docs
weight: 820
url: /ar/net/groupdocs.redaction/redactor/
---
## Redactor class

يمثل الفئة الرئيسية التي تتحكم في عملية حجب المستندات، وتسمح بفتح، حجب وحفظ المستندات.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | ينشئ مثيلاً جديداً من فئة [`Redactor`](../redactor) باستخدام تدفق بيانات. |
| [Redactor](redactor#constructor_3)(string) | ينشئ مثيلاً جديداً من فئة [`Redactor`](../redactor) باستخدام مسار ملف. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | ينشئ مثيلاً جديداً من فئة [`Redactor`](../redactor) لمستند محمي بكلمة مرور باستخدام تدفق بيانات. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | يُنشئ مثيلًا جديدًا من الفئة [`Redactor`](../redactor) لمستند محمي بكلمة مرور باستخدام مساره. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | يُنشئ مثيلًا جديدًا من الفئة [`Redactor`](../redactor) لمستند محمي بكلمة مرور باستخدام الدفق والإعدادات. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | يُنشئ مثيلًا جديدًا من الفئة [`Redactor`](../redactor) لمستند محمي بكلمة مرور باستخدام مساره والإعدادات. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | يطبق إخفاءً على المستند. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | يطبق سياسة إخفاء على المستند. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | يطبق مجموعة من الإخفاءات على المستند. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | يطلق الموارد. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | ينشئ صور معاينة لصفحات محددة بتنسيق صورة معين. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | يحصل على المعلومات العامة حول المستند - الحجم، عدد الصفحات، إلخ. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | يحفظ المستند إلى ملف. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | يحفظ المستند إلى الدفق المحدد. |

### ملاحظات

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### أمثلة

يوضح المثال التالي تطبيق إخفاء واحد على المستند.

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

يوضح المثال التالي تطبيق قائمة من الإخفاءات على المستند.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... إخفاءات أخرى
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false، إذا فشل إخفاء واحد على الأقل
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

يوضح المثال التالي كيفية تطبيق سياسة الإخفاء على جميع الملفات داخل مجلد الوارد المحدد، وحفظها في أحد مجلدات الصادر - للملفات التي تم تحديثها بنجاح وللملفات التي فشلت.

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

يوضح المثال التالي كيفية فتح مستندات محمية بكلمة مرور باستخدام LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // هنا يمكننا استخدام مثيل المستند لتنفيذ الإخفاءات
}
```

يوضح المثال التالي كيفية حفظ مستند باستخدام SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // هنا يتم تعديل المستند
       // ...
    
       // احفظ المستند باستخدام الخيارات الافتراضية (تحويل الصفحات إلى صور، حفظ كملف PDF)
       redactor.Save();
    
       // احفظ المستند بالتنسيق الأصلي مع استبدال الملف الأصلي
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // احفظ المستند إلى ملف "*_Redacted.*" بالتنسيق الأصلي
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // احفظ المستند إلى "*_AnyText.*" (مثلاً طابع زمني بدلاً من "AnyText") في اسم ملفه دون تحويل إلى نقطية
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### انظر أيضًا

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
