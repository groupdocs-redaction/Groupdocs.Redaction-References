---
title: IDocumentInfo
second_title: GroupDocs.Redaction لمرجع .NET API
description: يحدد الطرق المطلوبة للحصول على معلومات المستند الأساسية.
type: docs
weight: 100
url: /ar/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

يحدد الطرق المطلوبة للحصول على معلومات المستند الأساسية.

```csharp
public interface IDocumentInfo
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | يحصل على وصف تنسيق الملف. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | الحصول على إجمالي عدد الصفحات . |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | يحصل على قائمة[`PageInfo`](../pageinfo) معلومات الصفحة. |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | الحصول على حجم المستند بالبايت . |

### ملاحظات

**يتعلم أكثر**

* [احصل على معلومات الملف](https://docs.groupdocs.com/redaction/net/get-file-info/)

### أمثلة

يوضح المثال التالي كيفية استرداد معلومات المستند العامة باستخدام[`IDocumentInfo`](../idocumentinfo).

```csharp
    try
    {
        using (Redactor red = new Redactor(@"C:\Temp\testfile.doc"))
        {
            IDocumentInfo docInfo = red.GetDocumentInfo();
            Console.WriteLine("Document size: {0}", docInfo.Size);
            Console.WriteLine("Document format: {0}", docInfo.FileType.FileFormat);
            Console.WriteLine("Document contains {0} pages", docInfo.PageCount);
            foreach (PageInfo page in docInfo.Pages)
            {
                Console.WriteLine("Page {0} size is {1}x{2}", page.PageNumber, page.Width, page.Height);
            }
        }
    }
    catch (GroupDocs.Redaction.Exceptions.PasswordRequiredException)
    {
        Console.WriteLine("You are trying to access document which is password protected. Please, set the password.");
    }
    catch (GroupDocs.Redaction.Exceptions.IncorrectPasswordException)
    {
        Console.WriteLine("The provided password is not valid.");
    }
```

### أنظر أيضا

* مساحة الاسم [GroupDocs.Redaction](../../groupdocs.redaction)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->