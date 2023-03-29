---
title: PageInfo
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: एक संक्षप्त पृष्ठ जनकर क प्रतनधत्व करत है
type: docs
weight: 390
url: /hi/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

एक संक्षिप्त पृष्ठ जानकारी का प्रतिनिधित्व करता है।

```csharp
public class PageInfo
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageInfo](pageinfo)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | पृष्ठ ऊंचाई प्राप्त या सेट करता है। |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | पृष्ठ संख्या प्राप्त या सेट करता है। |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | पृष्ठ की चौड़ाई प्राप्त या सेट करता है। |

### टिप्पणियों

**और अधिक जानें**

* [फ़ाइल जानकारी प्राप्त करें](https://docs.groupdocs.com/redaction/net/get-file-info/)

### उदाहरण

निम्न उदाहरण दर्शाता है कि सामान्य दस्तावेज़ जानकारी का उपयोग करके कैसे पुनर्प्राप्त किया जाए[`IDocumentInfo`](../idocumentinfo).

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

### यह सभी देखें

* नाम स्थान [GroupDocs.Redaction](../../groupdocs.redaction)
* सभा [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->