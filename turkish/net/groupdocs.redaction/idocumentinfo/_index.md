---
title: "IDocumentInfo"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Temel belge bilgilerini almayı gerektiren yöntemleri tanımlar."
type: docs
weight: 100
url: /tr/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Temel belge bilgilerini almayı gerektiren yöntemleri tanımlar.

```csharp
public interface IDocumentInfo
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Dosya formatı açıklamasını alır. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Toplam sayfa sayısını alır. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | [`PageInfo`](../pageinfo) sayfa bilgilerinin listesini alır. |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Belgenin boyutunu bayt cinsinden alır. |

### Açıklamalar

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Örnekler

Aşağıdaki örnek, [`IDocumentInfo`](../idocumentinfo) kullanarak genel belge bilgilerini nasıl alacağını gösterir.

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

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
